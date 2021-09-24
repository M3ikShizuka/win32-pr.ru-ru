---
title: Примеры кода имеющуюся цепочку буферов композиции
description: Коллекция примеров кода, в которых показаны различные сценарии имеющуюся цепочку буферов композиции.
ms.topic: article
ms.date: 09/10/2021
ms.openlocfilehash: d538be46c6d41ed884ae9d4a735962317087e9c6
ms.sourcegitcommit: 2c13d0f1620f7c089687ef1d97e8c1d22e5d537a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "128524003"
---
# <a name="composition-swapchain-code-examples"></a>Примеры кода имеющуюся цепочку буферов композиции

> [!NOTE]
> **Некоторые сведения относятся к предварительной версии продукта, в которую перед коммерческим выпуском могут быть внесены существенные изменения. Корпорация Майкрософт не дает никаких гарантий, явных или подразумеваемых, в отношении предоставленной здесь информации.**

в этих примерах кода используются [библиотеки реализации Windows (будет)](https://github.com/Microsoft/wil). удобный способ установки будет — перейти к Visual Studio, щелкнуть **Project** \> **управление пакетами NuGet...** \> **обзор**, введите или вставьте **Microsoft. Windows. Имплементатионлибрари** в поле поиска выберите элемент в результатах поиска, а затем нажмите кнопку **установить** , чтобы установить пакет для этого проекта.

## <a name="example-1mdashcreating-a-presentation-manager-on-systems-that-support-the-composition-swapchain-api"></a>Пример 1. &mdash; Создание диспетчера презентаций на системах, поддерживающих API-интерфейс композиции имеющуюся цепочку буферов

Как уже упоминалось, для функционирования API композиции имеющуюся цепочку буферов требуются Поддерживаемые драйверы. В следующем примере показано, как приложение может создать диспетчер презентаций, если система поддерживает API. Это продемонстрировано в виде `TryCreate` функции в стиле, возвращающей диспетчер презентаций, только если API поддерживается. Эта функция также показывает, как правильно создать устройство Direct3D для резервного копирования диспетчера презентаций.

### <a name="c-example"></a>Пример C++

```cpp
bool TryCreatePresentationManager(
    _In_ bool requestDirectPresentation,
    _Out_ ID3D11Device** ppD3DDevice,
    _Outptr_opt_result_maybenull_ IPresentationManager **ppPresentationManager)
{
    // Null the presentation manager and Direct3D device initially
    *ppD3DDevice = nullptr;
    *ppPresentationManager = nullptr;

    // Direct3D device creation flags. The composition swapchain API requires that applications disable internal
    // driver threading optimizations, as these optimizations are incompatible with the
    // composition swapchain API. If this flag is not present, then the API will fail the call to create the
    // presentation factory.
    UINT deviceCreationFlags =
        D3D11_CREATE_DEVICE_BGRA_SUPPORT |
        D3D11_CREATE_DEVICE_SINGLETHREADED |
        D3D11_CREATE_DEVICE_PREVENT_INTERNAL_THREADING_OPTIMIZATIONS;

    // Create the Direct3D device.
    com_ptr_failfast<ID3D11DeviceContext> d3dDeviceContext;
    FAIL_FAST_IF_FAILED(D3D11CreateDevice(
        nullptr,                   // No adapter
        D3D_DRIVER_TYPE_HARDWARE,  // Hardware device
        nullptr,                   // No module
        deviceCreationFlags,       // Device creation flags
        nullptr, 0,                // Highest available feature level
        D3D11_SDK_VERSION,         // API version
        ppD3DDevice,               // Resulting interface pointer
        nullptr,                   // Actual feature level
        &d3dDeviceContext));       // Device context

    // Call the composition swapchain API export to create the presentation factory.
    com_ptr_failfast<IPresentationFactory> presentationFactory;
    FAIL_FAST_IF_FAILED(CreatePresentationFactory(
        (*ppD3DDevice),
        IID_PPV_ARGS(&presentationFactory)));

    // Determine whether the system is capable of supporting the composition swapchain API based
    // on the capability that's reported by the presentation factory. If your application
    // wants direct presentation (that is, presentation without the need for DWM to
    // compose, using MPO or iflip), then we query for direct presentation support.
    bool isSupportedOnSystem;
    if (requestDirectPresentation)
    {
        isSupportedOnSystem = presentationFactory->IsPresentationSupportedWithIndependentFlip();
    }
    else
    {
        isSupportedOnSystem = presentationFactory->IsPresentationSupported();
    }

    // Create the presentation manager if it is supported on the current system.
    if (isSupportedOnSystem)
    {
        FAIL_FAST_IF_FAILED(presentationFactory->CreatePresentationManager(ppPresentationManager));
    }

    return isSupportedOnSystem;
}
```

## <a name="example-2mdashcreating-a-presentation-manager-and-presentation-surface"></a>Пример 2. &mdash; Создание диспетчера презентаций и поверхности представления

В следующем примере показано, как приложение создает диспетчер презентаций и область презентации для привязки к визуальному элементу в визуальном дереве. в последующих примерах показано, как привязать поверхность презентации к визуальным деревьям [**DirectComposition**](/windows/win32/directcomp/directcomposition-portal) и [**Windows. UI. композиция**](/uwp/api/windows.ui.composition) .

### <a name="c-example-dcompositiongettargetstatistics"></a>Пример C++ (Дкомпоситионжеттаржетстатистикс)

```cpp
bool MakePresentationManagerAndPresentationSurface(
    _Out_ ID3D11Device** ppD3dDevice,
    _Out_ IPresentationManager** ppPresentationManager,
    _Out_ IPresentationSurface** ppPresentationSurface,
    _Out_ unique_handle& compositionSurfaceHandle)
{
    // Null the output pointers initially.
    *ppD3dDevice = nullptr;
    *ppPresentationManager = nullptr;
    *ppPresentationSurface = nullptr;
    compositionSurfaceHandle.reset();

    com_ptr_failfast<IPresentationManager> presentationManager;
    com_ptr_failfast<IPresentationSurface> presentationSurface;
    com_ptr_failfast<ID3D11Device> d3d11Device;

    // Call the function we defined previously to create a Direct3D device and presentation manager, if
    // the system supports it.
    if (TryCreatePresentationManager(
        true, // Request presentation with independent flip.
        &d3d11Device,
        &presentationManager) == false)
    {
        // Return 'false' out of the call if the composition swapchain API is unsupported. Assume the caller
        // will handle this somehow, such as by falling back to DXGI.
        return false;
    }

    // Use DirectComposition to create a composition surface handle.
    FAIL_FAST_IF_FAILED(DCompositionCreateSurfaceHandle(
        COMPOSITIONOBJECT_ALL_ACCESS,
        nullptr,
        compositionSurfaceHandle.addressof()));

    // Create presentation surface bound to the composition surface handle.
    FAIL_FAST_IF_FAILED(presentationManager->CreatePresentationSurface(
        compositionSurfaceHandle.get(),
        presentationSurface.addressof()));

    // Return the Direct3D device, presentation manager, and presentation surface to the caller for future
    // use.
    *ppD3dDevice = d3d11Device.detach();
    *ppPresentationManager = presentationManager.detach();
    *ppPresentationSurface = presentationSurface.detach();

    // Return 'true' out of the call if the composition swapchain API is supported and we were able to
    // create a presentation manager.
    return true;
}
```

## <a name="example-3mdashbinding-a-presentation-surface-to-a-windowsuicomposition-surface-brush"></a>пример 3 &mdash; . привязка области презентации к кисти Windows. UI. композиция

в следующем примере показано, как приложение привязывает маркер области композиции, привязанный к поверхности презентации, как показано в примере выше, к кисти [**Windows. UI. композиция**](/uwp/api/windows.ui.composition) (*винкомп*), которая затем может быть привязана к визуальному элементу sprite в визуальном дереве приложения.

### <a name="c-example"></a>Пример C++

```cpp
void BindPresentationSurfaceHandleToWinCompTree(
    _In_ ICompositor * pCompositor,
    _In_ ISpriteVisual * pVisualToBindTo, // The sprite visual we want to bind to.
    _In_ unique_handle& compositionSurfaceHandle)
{
    // QI an interop compositor from the passed compositor.
    com_ptr_failfast<ICompositorInterop> compositorInterop;
    FAIL_FAST_IF_FAILED(pCompositor->QueryInterface(IID_PPV_ARGS(&compositorInterop)));

    // Create a composition surface for the presentation surface's composition surface handle.
    com_ptr_failfast<ICompositionSurface> compositionSurface;
    FAIL_FAST_IF_FAILED(compositorInterop->CreateCompositionSurfaceForHandle(
        compositionSurfaceHandle.get(),
        &compositionSurface));

    // Create a composition surface brush, and bind the surface to it.
    com_ptr_failfast<ICompositionSurfaceBrush> surfaceBrush;
    FAIL_FAST_IF_FAILED(pCompositor->CreateSurfaceBrush(&surfaceBrush));
    FAIL_FAST_IF_FAILED(surfaceBrush->put_Surface(compositionSurface.get()));

    // Bind the brush to the visual.
    auto brush = surfaceBrush.query<ICompositionBrush>();
    FAIL_FAST_IF_FAILED(pVisualToBindTo->put_Brush(brush.get()));
}
```

## <a name="example-4mdashbinding-a-presentation-surface-to-a-directcomposition-visual"></a>Пример 4. &mdash; Привязка области презентации к визуальному элементу DirectComposition

В следующем примере показано, как приложение привязывает поверхность презентации к визуальному элементу DirectComposition (*дкомп*) в визуальном дереве.

### <a name="c-example"></a>Пример C++

```cpp
void BindPresentationSurfaceHandleToDCompTree(
    _In_ IDCompositionDevice* pDCompDevice,
    _In_ IDCompositionVisual* pVisualToBindTo,
    _In_ unique_handle& compositionSurfaceHandle) // The composition surface handle that was
                                                  // passed to CreatePresentationSurface.
{
    // Create a DComp surface to wrap the presentation surface.
    com_ptr_failfast<IUnknown> dcompSurface;
    FAIL_FAST_IF_FAILED(pDCompDevice->CreateSurfaceFromHandle(
        compositionSurfaceHandle.get(),
        &dcompSurface));

    // Bind the presentation surface to the visual.
    FAIL_FAST_IF_FAILED(pVisualToBindTo->SetContent(dcompSurface.get()));
}
```

## <a name="example-5mdashsetting-alpha-mode-and-color-space-on-a-presentation-surface"></a>Пример 5. &mdash; Настройка режима альфа и цветового пространства на поверхности презентации

В следующем примере показано, как приложение устанавливает режим альфа и цветовое пространство на поверхности презентации. Режим альфа описывает, следует ли интерпретировать альфа-канал в текстуре. Цветовое пространство описывает цветовое пространство, на которое ссылаются Пиксели текстуры.

Все подобные обновления свойств вступят в силу как часть следующего представления приложения и вступают в силу атомарно вместе с любыми обновлениями буфера, которые являются частью этого. Кроме того, это может быть, если ваше приложение захочет, не обновлять ни один буфер, а только обновления свойств. Все области представления, буферы которых не обновляются на определенном представлении, остаются привязанными к любому буферу, до которого они были привязаны.

### <a name="c-example"></a>Пример C++

```cpp
void SetAlphaModeAndColorSpace(
    _In_ IPresentationSurface* pPresentationSurface)
{
    // Set alpha mode.
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetAlphaMode(DXGI_ALPHA_MODE_IGNORE));

    // Set color space to full RGB.
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetColorSpace(DXGI_COLOR_SPACE_RGB_FULL_G22_NONE_P709));
}
```

## <a name="example-6mdashsetting-letterboxing-margins-on-a-presentation-surface"></a>Пример 6. &mdash; Установка пустых полей на поверхности презентации

В следующем примере показано, как приложение будет задавать пустых поля на поверхности презентации. Пустых используется для заполнения указанной области за пределами содержимого поверхности, чтобы учитывать различия пропорций содержимого и отображаемого устройства, на котором оно показано. Хорошим примером этого являются черные *полосы* , которые часто видны выше и под содержимым при просмотре на компьютере фильма, отформатированного для широкоэкранных кинотеатров. API-интерфейс композиции имеющуюся цепочку буферов позволяет указать поля, в которых должны отображаться пустых в таких случаях.

В настоящее время области пустых всегда заполняются непрозрачным черным цветом.

В виде содержимого визуального дерева поверхность презентации существует в пространстве координат своего визуального элемента. При наличии пустых источник пространства координат визуального элемента соответствует верхнему левому краю пустых. Это означает, что сам буфер находится в смещении на пространство координат визуального элемента. Границы вычисляются как размер буфера плюс размер пустых.

Ниже показано, где буфер и пустых существуют в визуальном пространстве координат и как вычисляются границы.

![Пустых поля](images/letterboxing-margins.png)

Наконец, если преобразование, применяемое к поверхности представления, сопровождается смещением, то область, не охватываемая буфером или пустых, считается вне границ содержимого и считается прозрачной, &mdash; аналогично тому, как любое другое содержимое визуального дерева обрабатывается вне границ содержимого.

### <a name="letterboxing-and-transform-interaction"></a>Взаимодействие пустых и Transform

Чтобы обеспечить единообразные размеры полей пустых независимо от масштаба, применяемого приложением к буферу для заполнения области содержимого, DWM попытается визуализировать поля по постоянному размеру независимо от масштаба, но принимая во внимание результат преобразования, примененного к поверхности презентации.

Другими словами, пустых поля технически применяются перед применением преобразования области представления, но можно компенсировать любой масштаб, который может быть частью этого преобразования. Это означает, что преобразование области презентации разбивается на два компонента, &mdash; часть которых масштабируется, и остаток преобразования.

![Взаимодействие пустых и Transform 1](images/letterboxing-and-transform-interaction-1.png)

Например, при использовании полей 100 пикс пустых и без преобразования к поверхности презентации результирующий буфер будет визуализирован без масштабирования, а пустых поля будут 100 пикс в ширину.

![Взаимодействие пустых и Transform 2](images/letterboxing-and-transform-interaction-2.png)

Еще один пример: с полями 100 пикс пустых и преобразованием масштаба 2x, примененным к поверхности презентации, результирующий буфер будет отображен с двукратным масштабированием, а пустых поля на экране будут по-прежнему иметь 100 пикс всех размеров.

![Взаимодействие пустых и Transform 3](images/letterboxing-and-transform-interaction-3.png)

Другой пример: при преобразовании с поворотом на 45 градусов результирующие пустых поля отобразятся 100 пикс, а пустых поля будут повернуты с помощью буфера.

![Взаимодействие пустых и Transform 4](images/letterboxing-and-transform-interaction-4.png)

Другой пример с преобразованием масштабирование 2x и поворот 45 градусов, изображение будет повернуто и масштабироваться, а пустых поля также будут 100 пиксы в ширину и будут поворачиваться с помощью буфера.

![Взаимодействие пустых и Transform 5](images/letterboxing-and-transform-interaction-5.png)

Если преобразование масштабирования не может быть однозначно извлечено из преобразования, которое приложение применяет к поверхности презентации, например, если итоговая шкала X или Y равна 0, то пустых поля будут подготавливаться ко всему преобразованию, и мы не будем пытаться компенсировать масштаб.

![Взаимодействие пустых и Transform 6](images/letterboxing-and-transform-interaction-6.png)

### <a name="c-example"></a>Пример C++

```cpp
 void SetContentLayoutAndFill(
    _In_ IPresentationSurface* pPresentationSurface)
{
    // Set layout properties. Each layout property is described below.

    // The source RECT describes the area from the bound buffer that will be sampled from. The
    // RECT is in source texture coordinates. Below we indicate that we'll sample from a
    // 100x100 area on the source texture.
    RECT sourceRect;
    sourceRect.left = 0;
    sourceRect.top = 0;
    sourceRect.right = 100;
    sourceRect.bottom = 100;
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetSourceRect(&sourceRect));

    // The presentation transform defines how the source rect will be transformed when
    // rendering the buffer. In this case, we indicate we want to scale it 2x in both
    // width and height, and we also want to offset it 50 pixels to the right.
    PresentationTransform transform = { 0 };
    transform.M11 = 2.0f; // X scale 2x
    transform.M22 = 2.0f; // Y scale 2x
    transform.M31 = 50.0f; // X offset 50px
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetTransform(&transform));

    // The letterboxing parameters describe how to letterbox the content. Letterboxing
    // is commonly used to fill area not covered by video/surface content when scaling to
    // an aspect ration that doesn't match the aspect ratio of the surface itself. For
    // example, when viewing content formatted for the theater on a 1080p home screen, one
    // can typically see black "bars" on the top and bottom of the video, covering the space
    // on screen that wasn't covered by the video due to the differing aspect ratios of the
    // content and the display device. The composition swapchain API allows the user to specify
    // letterboxing margins, which describe the number of pixels to surround the surface
    // content with on screen. In this case, surround the top and bottom of our content with
    // 100 pixel tall letterboxing.
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetLetterboxingMargins(
        0.0f,
        100.0f,
        0.0f,
        100.0f));
}
```

## <a name="example-7mdashsetting-content-restrictions-on-a-presentation-surface"></a>Пример 7. &mdash; Настройка ограничений на содержимое для поверхности презентации

В следующем примере показано, как ваше приложение запрещает другим приложениям считывать содержимое поверхности представления (от таких технологий, как принтскрин, ДДА, API захвата и др.), в целях защищенного содержимого. Здесь также показано, как ограничить отображение поверхности презентации только одним выходом DXGI.

Если содержимое реадбакк отключено, то когда приложение пытается выполнить чтение, захваченный образ будет содержать непрозрачный черный цвет вместо поверхности презентации. Если поверхность презентации ограничена [**идксгиаутпут**](/windows/win32/api/dxgi/nn-dxgi-idxgioutput), она будет отображаться как непрозрачный черный на всех остальных выходных данных.

### <a name="c-example"></a>Пример C++

```cpp
void SetContentRestrictions(
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ IDXGIOutput* pOutputToRestrictTo)
{
    // Disable readback of the surface via printscreen, bitblt, etc.
    FAIL_FAST_IF_FAILED(pPresentationSurface->SetDisableReadback(true));

    // Restrict display of surface to only the passed output.
    FAIL_FAST_IF_FAILED(pPresentationSurface->RestrictToOutput(pOutputToRestrictTo));
}
```

## <a name="example-8mdashadding-presentation-buffers-to-a-presentation-manager"></a>Пример 8. &mdash; Добавление буферов презентации в Диспетчер презентаций

В следующем примере показано, как приложение выделяет набор текстур Direct3D и добавляет их в Диспетчер презентаций для использования в качестве буферов презентации, которые могут быть представлены на поверхности представления.

Как уже упоминалось, не существует ограничений на количество руководителей презентаций, с которыми может быть зарегистрирована текстура. Однако в большинстве случаев текстура будет зарегистрирована только в одном диспетчере презентаций.

Также обратите внимание, что, поскольку API принимает дескрипторы общего буфера как валюту при регистрации текстур как буферов представления в диспетчере презентаций, а так как DXGI может создавать несколько общих буферов для одного texture2D, технически возможно, что приложение создает несколько дескрипторов общего буфера для одной текстуры и регистрирует их в диспетчере презентаций.  по сути, это повлияет на добавление одного и того же буфера несколько раз. Это не рекомендуется, так как оно нарушает механизмы синхронизации, предоставляемые диспетчером презентаций, так как два буфера презентации, которые отделены уникальным образом, фактически соответствуют одной и той же текстуре. Так как это расширенный API-интерфейс, и, поскольку в реализации он довольно трудно обнаружить, в этом случае API не пытается проверить этот сценарий.

### <a name="c-example"></a>Пример C++

```cpp
void AddBuffersToPresentationManager(
    _In_ ID3D11Device* pD3D11Device, // The backing Direct3D device
    _In_ IPresentationManager* pPresentationManager, // Previously-made presentation manager
    _In_ UINT bufferWidth, // The width of the buffers to add
    _In_ UINT bufferHeight, // The height of the buffers to add
    _In_ UINT numberOfBuffersToAdd, // The number of buffers to add to the presentation manager
    _Out_ vector<com_ptr_failfast<ID3D11Texture2D>>& textures, // Array of textures returned
    _Out_ vector<com_ptr_failfast<IPresentationBuffer>>& presentationBuffers) // Array of presentation buffers returned
{
    // Clear the returned vectors initially.
    textures.clear();
    presentationBuffers.clear();

    // Add the desired buffers to the presentation manager.
    for (UINT i = 0; i < numberOfBuffersToAdd; i++)
    {
        com_ptr_failfast<ID3D11Texture2D> texture;
        com_ptr_failfast<IPresentationBuffer> presentationBuffer;

        // Call our helper to make a new buffer of the desired type.
        AddNewPresentationBuffer(
            pD3D11Device,
            pPresentationManager,
            bufferWidth,
            bufferHeight,
            &texture,
            &presentationBuffer);

        // Track our buffers in our own set of vectors.
        textures.push_back(texture);
        presentationBuffers.push_back(presentationBuffer);
    }
}

void AddNewPresentationBuffer(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ UINT bufferWidth,
    _In_ UINT bufferHeight,
    _Out_ ID3D11Texture2D** ppTexture2D,
    _Out_ IPresentationBuffer** ppPresentationBuffer)
{
    com_ptr_failfast<ID3D11Texture2D> texture2D;
    unique_handle sharedResourceHandle;

    // Create a shared Direct3D texture and handle with the passed attributes.
    MakeD3D11Texture(
        pD3D11Device,
        bufferWidth,
        bufferHeight,
        &texture2D,
        out_param(sharedResourceHandle));

    // Add the texture2D to the presentation manager, and get back a presentation buffer.
    com_ptr_failfast<IPresentationBuffer> presentationBuffer;
    FAIL_FAST_IF_FAILED(pPresentationManager->AddBufferFromSharedHandle(
        sharedResourceHandle.get(),
        &presentationBuffer));

    // Return back the texture and buffer presentation buffer.
    *ppTexture2D = texture2D.detach();
    *ppPresentationBuffer = presentationBuffer.detach();
}

void MakeD3D11Texture(
    _In_ ID3D11Device* pD3D11Device,
    _In_ UINT textureWidth,
    _In_ UINT textureHeight,
    _Out_ ID3D11Texture2D** ppTexture2D,
    _Out_ HANDLE* sharedResourceHandle)
{
    D3D11_TEXTURE2D_DESC textureDesc = {};

    // Width and height can be anything within max texture size of the adapter backing the Direct3D
    // device.
    textureDesc.Width = textureWidth;
    textureDesc.Height = textureHeight;

    // MipLevels and ArraySize must be 1.
    textureDesc.MipLevels = 1;
    textureDesc.ArraySize = 1;

    // Format can be one of the following:
    //   DXGI_FORMAT_B8G8R8A8_UNORM
    //   DXGI_FORMAT_R8G8B8A8_UNORM
    //   DXGI_FORMAT_R16G16B16A16_FLOAT
    //   DXGI_FORMAT_R10G10B10A2_UNORM
    //   DXGI_FORMAT_NV12
    //   DXGI_FORMAT_YUY2
    //   DXGI_FORMAT_420_OPAQUE
    // For this 
    textureDesc.Format = DXGI_FORMAT_B8G8R8A8_UNORM;

    // SampleDesc count and quality must be 1 and 0 respectively.
    textureDesc.SampleDesc.Count = 1;
    textureDesc.SampleDesc.Quality = 0;

    // Usage must be D3D11_USAGE_DEFAULT.
    textureDesc.Usage = D3D11_USAGE_DEFAULT;

    // BindFlags must include D3D11_BIND_SHADER_RESOURCE for RGB textures, and D3D11_BIND_DECODER
    // for YUV textures. For RGB textures, it is likely your application will want to specify
    // D3D11_BIND_RENDER_TARGET in order to render to it.
    textureDesc.BindFlags =
        D3D11_BIND_SHADER_RESOURCE |
        D3D11_BIND_RENDER_TARGET;

    // MiscFlags should include D3D11_RESOURCE_MISC_SHARED and D3D11_RESOURCE_MISC_SHARED_NTHANDLE,
    // and might also include D3D11_RESOURCE_MISC_SHARED_DISPLAYABLE if your application wishes to
    // qualify for MPO and iflip. If D3D11_RESOURCE_MISC_SHARED_DISPLAYABLE is not provided, then the
    // content will not qualify for MPO or iflip, but can still be composed by DWM
    textureDesc.MiscFlags =
        D3D11_RESOURCE_MISC_SHARED |
        D3D11_RESOURCE_MISC_SHARED_NTHANDLE |
        D3D11_RESOURCE_MISC_SHARED_DISPLAYABLE;

    // CPUAccessFlags must be 0.
    textureDesc.CPUAccessFlags = 0;

    // Use Direct3D to create a texture 2D matching the desired attributes.
    com_ptr_failfast<ID3D11Texture2D> texture2D;
    FAIL_FAST_IF_FAILED(pD3D11Device->CreateTexture2D(&textureDesc, nullptr, &texture2D));

    // Create a shared handle for the texture2D.
    unique_handle sharedBufferHandle;
    auto dxgiResource = texture2D.query<IDXGIResource1>();
    FAIL_FAST_IF_FAILED(dxgiResource->CreateSharedHandle(
        nullptr,
        GENERIC_ALL,
        nullptr,
        &sharedBufferHandle));

    // Return the handle to the caller.
    *ppTexture2D = texture2D.detach();
    *sharedResourceHandle = sharedBufferHandle.release();
}
```

## <a name="example-9mdashremoving-presentation-buffers-from-a-presentation-manager-and-object-lifetime"></a>Пример 9. &mdash; Удаление буферов презентации из диспетчера презентаций и времени существования объектов

Удаление буфера презентации из диспетчера презентаций осуществляется так же просто, как освобождение объекта Ипресентатионбуффер на refcount 0. Однако в этом случае это не обязательно означает, что буфер презентации можно освободить. Возможны случаи, когда буфер по-прежнему используется, например, если этот буфер презентации виден на экране или содержит незавершенные представления, ссылающиеся на него.

Вкратце, диспетчер презентаций следит за тем, как каждый буфер используется приложением напрямую и косвенно. Он следит за тем, какие буферы отображаются, какие представления представляют собой необработанные и ссылочные буферы, а также внутренне отслеживает все это состояние, чтобы гарантировать, что буфер не будет полностью освобожден и не зарегистрирован, пока он не будет действительно использован.

Хорошим способом подумать о существовании буфера является то, что если приложение освобождает Ипресентатионбуффер, оно сообщает API, что он больше не будет использовать этот буфер во всех последующих вызовах. API композиции имеющуюся цепочку буферов будет отслеживать это, а также любые другие способы использования буфера, и он будет полностью освобождать буфер только в том случае, если это абсолютно надежно.

В коротком случае &mdash; приложение должно освободить [**ипресентатионбуффер**](/windows/win32/api/presentation/nn-presentation-ipresentationbuffer) , когда оно завершится с ним, а также ВЫЯСНИТЬ, что API композиции имеющуюся цепочку буферов будет полностью освобождать буфер, когда все остальные варианты использования будут завершены.

Ниже приведена иллюстрация описанных выше концепций.

![Удаление буферов презентации](images/removing-presentation-buffers.png)

В этом примере у нас есть диспетчер презентаций с двумя буферами презентации. В буфере 1 есть три ссылки, которые остаются в рабочем состоянии.

* Приложение содержит **ипресентатионбуффер** , ссылающееся на него.
* Внутри API он хранится в качестве текущего привязанного буфера области презентации, так как это последний буфер, привязанный к приложению, который затем был представлен.
* Кроме того, в текущей очереди есть необработанный ожидающий вывод буфера 1 на поверхности презентации.

Кроме того, буфер 1 содержит ссылку на соответствующее выделение текстуры Direct3D. У приложения также есть [**ID3D11Texture2D**](/windows/win32/api/d3d11/nn-d3d11-id3d11texture2d) , ссылающийся на это выделение.

В буфере 2 нет более необработанных ссылок со стороны приложения, а также не выполняется выделение текстуры, но буфер 2 сохраняется в активном состоянии, так как он отображается на экране в режиме презентации. Если имеется 1 обработка, а буфер 1 отображается на экране, буфер 2 будет иметь больше ссылок и будет освобожден, в свою очередь, чтобы освободить ссылку на его выделение Direct3D texture2D.

### <a name="c-example"></a>Пример C++

```cpp
void ReleasePresentationManagerBuffersExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager)
{
    com_ptr_failfast<ID3D11Texture2D> texture2D;
    com_ptr_failfast<IPresentationBuffer> newBuffer;

    // Create a new texture/presentation buffer.
    AddNewPresentationBuffer(
        pD3D11Device,
        pPresentationManager,
        200, // Buffer width
        200, // Buffer height
        &texture2D,
        &newBuffer);

    // Release the IPresentationBuffer. This indicates that we have no more intention to use it
    // from the application side. However, if we have any presents outstanding that reference
    // the buffer, it will be kept alive internally and released when all outstanding presents
    // have been retired.
    newBuffer.reset();

    // When the presentation buffer is truly released internally, it will in turn release its
    // reference on the texture2D which it corresponds to. Your application must also release
    // its own references to the texture2D for it to be released.
    texture2D.reset();
}
```

## <a name="example-10mdashresizing-buffers-in-a-presentation-manager"></a>Пример 10. &mdash; изменение размера буферов в диспетчере презентаций

В следующем примере показано, как приложение будет выполнять *изменение размера* буферов презентации. Например, если служба потоковой передачи Movie Streaming 480p, но решила переключить форматы в режим 1080p из-за доступности высокой пропускной способности сети, то потребуется перераспределить буферы из 480p в режим 1080p, чтобы он мог начать демонстрацию содержимого 1080p.

В DXGI это называется операцией *изменения размера* . В режиме DXGI все буферы перераспределяются атомарно, что является дорогостоящим и может вызвать сбой на экране. В этом примере описывается, как добиться атомарного изменения размера по номиналу с помощью DXGI в API-интерфейсе композиции имеющуюся цепочку буферов. В следующем примере показано, как изменить размер в горизонтальном *порядке* , изменяя распределение между несколькими представлениями, обеспечивая лучшую производительность, чем атомарный имеющуюся цепочку буферов.

### <a name="c-example"></a>Пример C++

```cpp
void ResizePresentationManagerBuffersExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager) // Previously-made presentation manager.
{
    // Vectors representing the IPresentationBuffer and ID3D11Texture2D collections.
    vector<com_ptr_failfast<ID3D11Texture2D>> textures;
    vector<com_ptr_failfast<IPresentationBuffer>> presentationBuffers;

    // Add 6 50x50 buffers to the presentation manager. See previous example for definition of
    // this function.
    AddBuffersToPresentationManager(
        pD3D11Device,
        pPresentationManager,
        50, // Buffer width
        50, // Buffer height
        6, // Number of buffers
        textures,
        presentationBuffers);

    // Release all the buffers we just added. The presentation buffers internally will be released
    // when any other references are also removed (outstanding presents, display references, etc.).
    textures.clear();
    presentationBuffers.clear();

    // Add 6 new 100x100 buffers to the presentation manager to replace the
    // old ones we just removed.
    AddBuffersToPresentationManager(
        pD3D11Device,
        pPresentationManager,
        100, // Buffer width
        100, // Buffer height
        6, // Number of buffers
        textures,
        presentationBuffers);
}
```

## <a name="example-11mdashsynchronizing-presentation-using-buffer-available-events-and-handling-presentation-manager-lost-events"></a>Пример 11. &mdash; Синхронизация презентации с использованием буфера доступных событий и обработка потерянных событий диспетчера презентаций

Если ваше приложение будет выдавать представление, включающее буфер презентации, который использовался ранее, то необходимо убедиться, что предыдущая Презентация завершена для повторной визуализации и представления буфера презентации. API-интерфейс композиции имеющуюся цепочку буферов предоставляет несколько различных механизмов для упрощения синхронизации. Самый простой — это *событие доступного* буфера презентации, которое является объектом события NT, сообщающим, когда буфер доступен для использования (т. е. во всех предыдущих представлениях введено либо снятие *с учета, либо* *упраздненное* состояние), а в противном случае — несигнальное. В этом примере показано, как использовать доступные в буфере события для выбора доступных буферов для представления. Здесь также показано, как прослушивать ошибки *потерянных устройств* , которые в точности эквивалентны потере устройства DXGI, и потребовать воссоздание диспетчера презентаций.

### <a name="presentation-manager-lost-errors"></a>Диспетчер презентаций потерял ошибки

Диспетчер презентаций может стать потерянным, если обнаруживает ошибку внутренним образом, которая не может быть восстановлена из. Приложение должно уничтожить утерянный диспетчер презентаций и создать новый, чтобы использовать его. Когда диспетчер презентаций теряется, он перестанет принимать дальнейшие представления. Любая попытка вызвать **Present** в утерянном диспетчере презентаций возвратит **PRESENTATION_ERROR_LOST**. Однако все остальные методы будут работать нормально. Это необходимо для того, чтобы приложение должно было только проверять наличие **PRESENTATION_ERROR_LOST** в существующих вызовах и не требуется ожидать или обработайте потерянные ошибки при каждом вызове API. Если приложение должно проверять или получать уведомления о потерянных ошибках за пределами текущего вызова, оно может использовать событие Lost, возвращенное [**ипресентатионманажер:: жетлостевент**](/windows/win32/api/presentation/nf-presentation-ipresentationmanager-getlostevent).

### <a name="present-queue-and-timing"></a>Представление очереди и времени

Представления, выданные диспетчером презентаций, могут указывать конкретное время назначения. Это конечное время — идеальное время, в течение которого система попытается отобразить текущее значение. Так как экраны обновляются с ограниченной частотой, присутствие вряд ли будет отображаться точно в указанное время, но оно отобразится как можно ближе к времени.

Это целевое время — относительно системы, или время, когда система была запущена с момента включения, в единицах, прошедших сотни наносекунд. Простой способ вычисления текущего времени — запросить текущее значение [**QueryPerformanceCounter**](/windows/win32/api/profileapi/nf-profileapi-queryperformancecounter) (QPC), разделить его на частоту QPC системы и умножить его на 10 000 000. Ограничения округления и точности в сторону это значение будет вычислять текущее время в соответствующих единицах. Система также может получить текущее время, вызвав [**мфжетсистемтиме**](/windows/win32/api/mfidl/nf-mfidl-mfgetsystemtime)или [**куеринтеррупттимепреЦисе**](/windows/win32/api/realtimeapiset/nf-realtimeapiset-queryinterrupttimeprecise).

После того как текущее время известно, ваше приложение обычно выдает по возрастанию смещений от текущего времени.

Независимо от целевого времени, представление всегда обрабатывается в порядке очередей. Даже если объект находится в более раннем времени, чем предыдущий, он не будет обработан до тех пор, пока не будут обработаны эти предыдущие представления. По сути, это означает, что любое присутствие, которое не нацелено на более позднее время, чем оно будет переопределено ранее. Это также означает, что если вашему приложению нужно *как можно раньше* выпустить представление, то оно может просто не задавать целевое время (в этом случае целевое время останется в том, что было в последний раз), или задать целевое время 0. Оба будут иметь одинаковый результат. Если приложению не нужно ждать, пока не будет завершено предыдущее представление, то потребуется отменить предыдущие представления. В следующем примере описывается, как это сделать.

![Представление очереди и времени](images/present-queue-and-timing.png)

**T = 3S**: Present 1, 2, 3 все готово, а 3 — Последнее присутствие, WINS. **T = 4S**: присутствие 4, 5, 6 всех готовых и 6, Последнее присутствие: WINS.

На приведенной выше схеме показан пример необработанных данных, представленных в текущей очереди. Present 1 предназначено для времени 3S. Таким образом, никакие выводятся до 3S. Однако присутствие 2 на самом деле нацелено на более раннее время, 1 – 2, а также на три мишени 3S. Таким образом, в момент времени 3S предоставляет 1, 2 и 3 все завершенные, и представление 3 будет фактически применено. После этого, приведенный ниже 4, будет удовлетворен на 4S, но сразу же переопределится на 5, где наследуется число 0, которое наследуется на 0, и в нем будет 6, для которого не задано целевое время. 5 и 6 вступают *в силу как можно раньше*.

### <a name="c-example"></a>Пример C++

```cpp
bool SimpleEventSynchronizationExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ vector<com_ptr_failfast<ID3D11Texture2D>>& textures,
    _In_ vector<com_ptr_failfast<IPresentationBuffer>>& presentationBuffers)
{
    // Track a time we'll be presenting to below. Default to the current time, then increment by
    // 1/10th of a second every present.
    SystemInterruptTime presentTime;
    QueryInterruptTimePrecise(&presentTime.value);

    // Build an array of events that we can wait on to perform various actions in our work loop.
    vector<unique_event> waitEvents;

    // The lost event will be the first event in our list. This is an event that signifies that
    // something went wrong in the system (due to extreme conditions such as memory pressure, or
    // driver issues) that indicate that the presentation manager has been lost, and should no
    // longer be used, and instead should be recreated.
    unique_event lostEvent;
    pPresentationManager->GetLostEvent(&lostEvent);
    waitEvents.emplace_back(std::move(lostEvent));

    // Add each buffer's available event to the list of events we will be waiting on.
    for (UINT bufferIndex = 0; bufferIndex < presentationBuffers.size(); bufferIndex++)
    {
        unique_event availableEvent;
        presentationBuffers[bufferIndex]->GetAvailableEvent(&availableEvent);
        waitEvents.emplace_back(std::move(availableEvent));
    }

    // Iterate for 120 presents.
    constexpr UINT numberOfPresents = 120;
    for (UINT onPresent = 0; onPresent < numberOfPresents; onPresent++)
    {
        // Advance our present time 1/10th of a second in the future. Note the API accepts
        // time in 100ns units, or 1/1e7 of a second, meaning that 1 million units correspond to
        // 1/10th of a second.
        presentTime.value += 1'000'000;

        // Wait for the lost event or an available buffer. Since WaitForMultipleObjects prioritizes
        // lower-indexed events, it is recommended to put any higher importance events (like the
        // lost event) first, and then follow up with buffer available events.
        DWORD waitResult = WaitForMultipleObjects(
            static_cast<UINT>(waitEvents.size()),
            reinterpret_cast<HANDLE*>(waitEvents.data()),
            FALSE,
            INFINITE);

        // Failfast if the wait hit an error.
        FAIL_FAST_IF((waitResult - WAIT_OBJECT_0) >= waitEvents.size());

        // Our lost event was the first event in the array. If this is signaled, the caller
        // should recreate the presentation manager. This is very similar to how Direct3D devices
        // can be lost. Assume our caller knows to handle this return value appropriately.
        if (waitResult == WAIT_OBJECT_0)
        {
            return false;
        }

        // Otherwise, compute the buffer corresponding to the available event that was signaled.
        UINT bufferIndex = waitResult - (WAIT_OBJECT_0 + 1);

        // Draw red to that buffer
        DrawColorToSurface(
            pD3D11Device,
            textures[bufferIndex],
            1.0f, // red
            0.0f, // green
            0.0f); // blue

        // Bind the presentation buffer to the presentation surface. Changes in this binding will take
        // effect on the next present, and the binding persists across presents. That is, any number
        // of subsequent presents will imply this binding until it is changed. It is completely fine
        // to only update buffers for a subset of the presentation surfaces owned by a presentation
        // manager on a given present - the implication is that it simply didn't update.
        //
        // Similarly, note that if your application were to call SetBuffer on the same presentation
        // surface multiple times without calling present, this is fine. The policy is last writer
        // wins.
        //
        // Your application may present without first binding a presentation surface to a buffer.
        // The result will be that presentation surface will simply have no content on screen,
        // similar to how DComp and WinComp surfaces appear in a tree before they are rendered to.
        // In that case system content will show through where the buffer would have been.
        //
        // Your application may also set a 'null' buffer binding after previously having bound a
        // buffer and present - the end result is the same as if your application had presented
        // without ever having set the content.
        pPresentationSurface->SetBuffer(presentationBuffers[bufferIndex].get());

        // Present at the targeted time. Note that a present can target only a single time. If an
        // application wants to updates two buffers at two different times, then it must present
        // two times.
        //
        // Presents are always processed in queue order. A present will not take effect before any
        // previous present in the queue, even if it targets an earlier time. In such a case, when
        // the previous present is processed, the next present will also be processed immediately,
        // and override that previous present.
        //
        // For this reason, if your application wishes to present "now" or "early as possible", then
        // it can simply present, without setting a target time. The implied target time will be 0,
        // and the new present will override the previous present.
        //
        // If your application wants to present truly "now", and not wait for previous presents in the
        // queue to be processed, then it will need to cancel previous presents. A future example
        // demonstrates how to do this.
        //
        // Your application will receive PRESENTATION_ERROR_LOST if it attempts to Present a lost
        // presentation manager. This is the only call that will return such an error. A lost
        // presentation manager functions normally in every other case, so applications need only
        // to handle this error at the time they call Present.
        pPresentationManager->SetTargetTime(presentTime);
        HRESULT hrPresent = pPresentationManager->Present();
        if (hrPresent == PRESENTATION_ERROR_LOST)
        {
            // Our presentation manager has been lost. Return 'false' to the caller to indicate that
            // the presentation manager should be recreated.
            return false;
        }
        else
        {
            FAIL_FAST_IF_FAILED(hrPresent);
        }
    }

    return true;
}

void DrawColorToSurface(
    _In_ ID3D11Device* pD3D11Device,
    _In_ const com_ptr_failfast<ID3D11Texture2D>& texture2D,
    _In_ float redValue,
    _In_ float greenValue,
    _In_ float blueValue)
{
    com_ptr_failfast<ID3D11DeviceContext> D3DDeviceContext;
    com_ptr_failfast<ID3D11RenderTargetView> renderTargetView;

    // Get the immediate context from the D3D11 device.
    pD3D11Device->GetImmediateContext(&D3DDeviceContext);

    // Create a render target view of the passed texture.
    auto resource = texture2D.query<ID3D11Resource>();
    FAIL_FAST_IF_FAILED(pD3D11Device->CreateRenderTargetView(
        resource.get(),
        nullptr,
        renderTargetView.addressof()));

    // Clear the texture with the specified color.
    float clearColor[4] = { redValue, greenValue, blueValue, 1.0f }; // red, green, blue, alpha
    D3DDeviceContext->ClearRenderTargetView(renderTargetView.get(), clearColor);
}
```

## <a name="example-12mdashadvanced-synchronizationmdashthrottling-workflow-to-the-size-of-the-outstanding-present-queue-using-present-synchronization-fences-and-handling-presentation-manager-lost-events"></a>Пример 12. &mdash; Расширенный &mdash; Рабочий процесс регулирования синхронизации до размера необработанной очереди на основе существующих ограждений синхронизации и обработки потерянных событий диспетчера презентаций

В следующем примере показано, как ваше приложение может отправить большое количество запросов в будущем, а затем спать до тех пор, пока не будет представлено количество невыполненных попадений на определенное количество. такие платформы, как Windows, Media Foundation регулировать этот способ, чтобы сократить количество пропусков цп, и при этом гарантировать, что текущая очередь не будет исчерпана (что помешает плавному воспроизведению и вызвать сбой). Это влияет на минимизацию потребления ресурсов ЦП во время рабочего процесса презентации. Приложение будет ставить в очередь максимальное количество презентаций (в зависимости от числа выделенных буферов презентации), а затем ждать до тех пор, пока очередь не будет исчерпана.

### <a name="c-example"></a>Пример C++

```cpp
bool FenceSynchronizationExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ vector<com_ptr_failfast<ID3D11Texture2D>>& textures,
    _In_ vector<com_ptr_failfast<IPresentationBuffer>>& presentationBuffers)
{
    // Track a time we'll be presenting to below. Default to the current time, then increment by
    // 1/10th of a second every present.
    SystemInterruptTime presentTime;
    QueryInterruptTimePrecise(&presentTime.value);

    // Get present retiring fence.
    com_ptr_failfast<ID3D11Fence> presentRetiringFence;
    FAIL_FAST_IF_FAILED(pPresentationManager->GetPresentRetiringFence(
        IID_PPV_ARGS(&presentRetiringFence)));

    // Get the lost event to query before presentation.
    unique_event lostEvent;
    pPresentationManager->GetLostEvent(&lostEvent);

    // Create an event to synchronize to our queue depth with. We'll use Direct3D to signal this event
    // when our synchronization fence indicates reaching a specific present.
    unique_event presentQueueSyncEvent;
    presentQueueSyncEvent.create(EventOptions::ManualReset);

    // Cycle the present queue 10 times.
    constexpr UINT numberOfPresentRefillCycles = 10;
    for (UINT onRefillCycle = 0; onRefillCycle < numberOfPresentRefillCycles; onRefillCycle++)
    {
        // Fill up presents for all presentation buffers. We compare the presentation manager's
        // next present ID to the present confirmed fence's value to figure out how
        // far ahead we are. We stop when we've issued presents for all buffers.
        while ((pPresentationManager->GetNextPresentId() -
                presentRetiringFence->GetCompletedValue()) < presentationBuffers.size())
        {
            // Present buffers in cyclical pattern. We can figure out the current buffer to
            // present by taking the modulo of the next present ID by the number of buffers. Note that the
            // first present of a presentation manager always has a present ID of 1 and increments by 1 on
            // each subsequent present. A present ID of 0 is conceptually meant to indicate that "no
            // presents have taken place yet".
            UINT bufferIndex = static_cast<UINT>(
                pPresentationManager->GetNextPresentId() % presentationBuffers.size());

            // Assert that the passed buffer is tracked as available for presentation. Because we throttle
            // based on the total number of buffers, this should always be true.
            NT_ASSERT(presentationBuffers[bufferIndex]->IsAvailable());

            // Advance our present time 1/10th of a second in the future.
            presentTime.value += 1'000'000;

            // Draw red to the texture.
            DrawColorToSurface(
                pD3D11Device,
                textures[bufferIndex],
                1.0f, // red
                0.0f, // green
                0.0f); // blue

            // Bind the presentation buffer to the presentation surface.
            pPresentationSurface->SetBuffer(presentationBuffers[bufferIndex].get());

            // Present at the targeted time.
            pPresentationManager->SetTargetTime(presentTime);
            HRESULT hrPresent = pPresentationManager->Present();
            if (hrPresent == PRESENTATION_ERROR_LOST)
            {
                // Our presentation manager has been lost. Return 'false' to the caller to indicate that
                // the presentation manager should be recreated.
                return false;
            }
            else
            {
                FAIL_FAST_IF_FAILED(hrPresent);
            }
        };

        // Now that the buffer is full, go to sleep until the present queue has been drained to
        // the desired queue depth. To figure out the appropriate present to wake on, we subtract
        // the desired wake queue depth from the presentation manager's last present ID. We
        // use Direct3D's SetEventOnCompletion to signal our wait event when that particular present
        // is retiring, and then wait on that event. Note that the semantic of SetEventOnCompletion
        // is such that even if we happen to call it after the fence has already reached the
        // requested value, the event will be set immediately.
        constexpr UINT wakeOnQueueDepth = 2;
        presentQueueSyncEvent.ResetEvent();
        FAIL_FAST_IF_FAILED(presentRetiringFence->SetEventOnCompletion(
            pPresentationManager->GetNextPresentId() - 1 - wakeOnQueueDepth,
            presentQueueSyncEvent.get()));

        HANDLE waitHandles[] = { lostEvent.get(), presentQueueSyncEvent.get() };
        DWORD waitResult = WaitForMultipleObjects(
            ARRAYSIZE(waitHandles),
            waitHandles,
            FALSE,
            INFINITE);

        // Failfast if we hit an error during our wait.
        FAIL_FAST_IF((waitResult - WAIT_OBJECT_0) >= ARRAYSIZE(waitHandles));

        if (waitResult == WAIT_OBJECT_0)
        {
            // The lost event was signaled - return 'false' to the caller to indicate that
            // the presentation manager was lost.
            return false;
        }

        // Iterate into another refill cycle.
    }

    return true;
}
```

## <a name="example-13mdashvsync-interrupts-and-hardware-flip-queue-support"></a>Пример 13 &mdash; вертикальной синхронизации прерываний и поддержка очереди аппаратного отражения

Наряду с этим API появилась новая форма «Управление очередями», называемая *очередью зеркального отражения оборудования* , что позволяет оборудованию GPU полностью работать независимо от ЦП. Основное преимущество этого подхода заключается в эффективности энергопотребления. Если ЦП не требуется участвовать в процессе презентации, будет выводиться меньше энергии.

Недостатком того, что обработчик GPU представляется независимо, является то, что состояние ЦП больше не может сразу отражаться при отображении представлений. концепции API композиции имеющуюся цепочку буферов, такие как доступные в буфере события, границы синхронизации и текущая статистика, не будут немедленно обновлены. Вместо этого GPU будет обновляться только периодическое состояние ЦП в соответствии с отображаемыми сведениями. Это означает, что обратная связь для приложений, касающихся текущего состояния, будет поступать с задержкой.

Как правило, приложение позаботится о том, что некоторые из них показывают, но не очень важны для других. Например, если в приложении выдается 10, это может решить, что он хочет узнать о том, что 8-й пример отображается, поэтому он может снова начать повторное заполнение очереди. В этом случае единственное, что действительно требуется для получения отзыва, — это восьмой момент. При отображении 1-7 или 9 не планируется ничего делать.

Определяет, будет ли состояние ЦП обновления зависеть от того, настроено ли оборудование GPU для создания прерывания вертикальной синхронизации при его наличии. Это вертикальной синхронизации прерывание ведет к запуску ЦП, если он еще не активен, а процессор запустит Специальный код уровня ядра для обновления себя в тех представлениях, которые произошли на GPU с момента последней проверки, в свою очередь, в том числе обновление механизмов обратной связи, таких как события буфера, текущая граница снятия с учета и вывод статистики.

Чтобы позволить приложению явно указать, какие представления должны выдавать прерывание вертикальной синхронизации, диспетчер презентаций предоставляет метод [**ипресентатионманажер:: форцевсинЦинтеррупт**](/windows/win32/api/presentation/nf-presentation-ipresentationmanager-forcevsyncinterrupt) , указывающий, должен ли следующий объект выдавать прерывание вертикальной синхронизации. Этот параметр применяется ко всем фьючерсам до тех пор, пока он не изменится, подобно [**ипресентатионманажер:: сеттаржеттиме**](/windows/win32/api/presentation/nf-presentation-ipresentationmanager-settargettime) и [**Ипресентатионманажер:: сетпреферредпресентдуратион**](/windows/win32/api/presentation/nf-presentation-ipresentationmanager-setpreferredpresentduration).

Если этот параметр включен в определенном месте, то оборудование немедленно уведомляет ЦП при его наличии, используя больше энергии, но гарантируя, что ЦП немедленно уведомляется о том, что происходит в настоящее время, чтобы приложения могли максимально быстро реагировать на запросы. Если этот параметр отключен на определенном компьютере, то система будет разрешать обновление ЦП при &mdash; сохранении питания, но отменяет отзыв.

Как правило, приложение не будет принудительно вызывать прерывание вертикальной синхронизации для любого представления, за исключением того, что он хочет синхронизироваться с. В приведенном выше примере, так как ваше приложение должно было пробудиться при отображении 8-го представления очереди, оно запросит, что в настоящее время 8 сигнализирует о вертикальной синхронизации прерывании, но в нем содержится 1-7 и 9. 

По умолчанию, если приложение не настраивает этот параметр, диспетчер презентаций всегда будет указывать прерывание вертикальной синхронизации при каждом отображении. Приложения, которые не интересуются энергопотреблением или не знают о поддержке очереди отражения оборудования, могут просто не вызывать **форцевсинЦинтеррупт**, и они гарантированно будут правильно синхронизироваться в результате. Приложения, осведомленные о поддержке очереди отражения оборудования, могут явно управлять этим параметром для повышения эффективности энергопотребления.

Ниже приведена схема, описывающая поведение API в отношении параметров прерывания вертикальной синхронизации.

![Прерывания вертикальной синхронизации](images/vsync-interrupts.png)

### <a name="c-example"></a>Пример C++

```cpp
bool ForceVSyncInterruptPresentsExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ vector<com_ptr_failfast<ID3D11Texture2D>>& textures,
    _In_ vector<com_ptr_failfast<IPresentationBuffer>>& presentationBuffers)
{
    // Track a time we'll be presenting to below. Default to the current time, then increment by
    // 1/10th of a second every present.
    SystemInterruptTime presentTime;
    QueryInterruptTimePrecise(&presentTime.value);

    // Get present retiring fence.
    com_ptr_failfast<ID3D11Fence> presentRetiringFence;
    FAIL_FAST_IF_FAILED(pPresentationManager->GetPresentRetiringFence(
        IID_PPV_ARGS(&presentRetiringFence)));

    // Get the lost event to query before presentation.
    unique_event lostEvent;
    pPresentationManager->GetLostEvent(&lostEvent);

    // Create an event to synchronize to our queue depth with. We will use Direct3D to signal this event
    // when our synchronization fence indicates reaching a specific present.
    unique_event presentQueueSyncEvent;
    presentQueueSyncEvent.create(EventOptions::ManualReset);

    // Issue 10 presents, and wake when the present queue is 2 entries deep (which happens when
    // present 7 is retiring).
    constexpr UINT wakeOnQueueDepth = 2;
    constexpr UINT numberOfPresents = 10;
    const UINT presentIdToWakeOn = numberOfPresents - 1 - wakeOnQueueDepth;
    while (pPresentationManager->GetNextPresentId() <= numberOfPresents)
    {
        UINT bufferIndex = static_cast<UINT>(
            pPresentationManager->GetNextPresentId() % presentationBuffers.size());

        // Advance our present time 1/10th of a second in the future.
        presentTime.value += 1'000'000;

        // Draw red to the texture.
        DrawColorToSurface(
            pD3D11Device,
            textures[bufferIndex],
            1.0f, // red
            0.0f, // green
            0.0f); // blue

        // Bind the presentation buffer to the presentation surface.
        pPresentationSurface->SetBuffer(presentationBuffers[bufferIndex].get());

        // Present at the targeted time.
        pPresentationManager->SetTargetTime(presentTime);

        // If this present is not going to retire the present that we want to wake on when it is shown, then
        // we don't need immediate updates to buffer available events, present retiring fence, or present
        // statistics. As such, we can mark it as not requiring a VSync interrupt, to allow for greater
        // power efficiency on machines with hardware flip queue support.
        bool forceVSyncInterrupt = (pPresentationManager->GetNextPresentId() == (presentIdToWakeOn + 1));
        pPresentationManager->ForceVSyncInterrupt(forceVSyncInterrupt);

        HRESULT hrPresent = pPresentationManager->Present();
        if (hrPresent == PRESENTATION_ERROR_LOST)
        {
            // Our presentation manager has been lost. Return 'false' to the caller to indicate that
            // the presentation manager should be recreated.
            return false;
        }
        else
        {
            FAIL_FAST_IF_FAILED(hrPresent);
        }
    }

    // Now that the buffer is full, go to sleep until presentIdToWakeOn has begun retiring. We
    // configured the subsequent present to force a VSync interrupt when it is shown, which will ensure
    // this wait is completed immediately.
    presentQueueSyncEvent.ResetEvent();
    FAIL_FAST_IF_FAILED(presentRetiringFence->SetEventOnCompletion(
        presentIdToWakeOn,
        presentQueueSyncEvent.get()));

    HANDLE waitHandles[] = { lostEvent.get(), presentQueueSyncEvent.get() };
    DWORD waitResult = WaitForMultipleObjects(
        ARRAYSIZE(waitHandles),
        waitHandles,
        FALSE,
        INFINITE);

    // Failfast if we hit an error during our wait.
    FAIL_FAST_IF((waitResult - WAIT_OBJECT_0) >= ARRAYSIZE(waitHandles));

    if (waitResult == WAIT_OBJECT_0)
    {
        // The lost event was signaled - return 'false' to the caller to indicate that
        // the presentation manager was lost.
        return false;
    }

    return true;
}
```

## <a name="example-14mdashcanceling-presents-scheduled-for-the-future"></a>Пример 14. &mdash; Отмена отменяемых утверждений в будущем

Приложения мультимедиа, которые в будущем представляют собой очередь, могут решить, что они уже были выпущены ранее. Это может произойти, например, если приложение воспроизводит видео, выдавало большое количество кадров в будущем, и пользователь решает приостановить воспроизведение видео. В этом случае приложение будет захотеть перейти к текущему кадру и отменить все последующие кадры, которые еще не были поставлены в очередь. Это также может произойти, если приложение мультимедиа принимает решение о перемещении воспроизведения в другую точку видео. В этом случае приложение будет отменять все, что еще не помещается в очередь на старое место в видео, и заменит их на новое место. В этом случае после отмены предыдущего примера приложение может выдать новое представление в будущем, соответствующее новой точке видео.

### <a name="c-example"></a>Пример C++

```cpp
void PresentCancelExample(
    _In_ IPresentationManager* pPresentationManager,
    _In_ UINT64 firstPresentIDToCancelFrom)

{
    // Assume we've issued a number of presents in the future. Something happened in the app, and
    // we want to cancel the issued presents that occur after a specified time or present ID. This
    // may happen, for example, when the user pauses playback from inside a media application. The
    // application will want to cancel all presents posted targeting beyond the pause time. The
    // cancel will apply to all previously posted presents whose present IDs are at least
    // 'firstPresentIDToCancelFrom'. Note that Present IDs are always unique, and never recycled,
    // so even if a present is canceled, no subsequent present will ever reuse its present ID.
    //
    // Also note that if some presents we attempt to cancel can't be canceled because they've
    // already started queueing, then no error will be returned, they simply won't be canceled as
    // requested. Cancelation takes a "best effort" approach.
    FAIL_FAST_IF_FAILED(pPresentationManager->CancelPresentsFrom(firstPresentIDToCancelFrom));

    // In the case where the media application scrubbed to a different position in the video, it may now
    // choose to issue new presents to replace the ones canceled. This is not illustrated here, but
    // previous examples that demonstrate presentation show how this may be achieved.
}
```

## <a name="example-15mdashstaggered-buffer-resize-operation-for-improved-performance"></a>Пример 15. &mdash; операция изменения размера буфера в шахматном порядке для повышения производительности

В этом примере показано, как приложение может разнести изменения в размер буфера для повышения производительности через DXGI. Припомните наш предыдущий пример изменения размера, где клиент службы потоковой передачи фильмов хочет изменить разрешение воспроизведения с 720p на 1080p. В DXGI приложение будет выполнять операцию изменения размера для имеющуюся цепочку буферов DXGI, что привело бы к неравномерному выдаче всех предыдущих буферов и повторно распределять все новые буферы 1080p и добавлять их в имеющуюся цепочку буферов. Этот тип атомарного изменения размера буферов является дорогостоящим и может занять много времени и вызвать сбой. Новый API обеспечивает более точный контроль над отдельными буферами представления. Таким образом, буферы могут быть перераспределены и заменены один на один в нескольких случаях для разделения рабочей нагрузки с течением времени. Это оказывает меньшее влияние на любой из существующих и гораздо менее вероятно приводит к возникновению сбоев. По сути, для диспетчера презентаций с n буферами презентации в представлении "n" приложение может удалить старый буфер презентации со старым размером, выделить новый буфер презентации на новом размере и показать его. После того как n будет представлено, все буферы будут иметь новый размер.

### <a name="c-example"></a>Пример C++

```cpp
bool StaggeredResizeExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ vector<com_ptr_failfast<ID3D11Texture2D>> textures,
    _In_ vector<com_ptr_failfast<IPresentationBuffer>> presentationBuffers)
{
    // Track a time we'll be presenting to below. Default to the current time, then increment by
    // 1/10th of a second every present.
    SystemInterruptTime presentTime;
    QueryInterruptTimePrecise(&presentTime.value);

    // Assume textures/presentationBuffers vector contains 10 100x100 buffers, and we want to resize
    // our swapchain to 200x200. Instead of reallocating 10 200x200 buffers all at once,
    // like DXGI does today, we can stagger the reallocation across multiple presents. For
    // each present, we can allocate one buffer at the new size, and replace one old buffer
    // at the old size with the new one at the new size. After 10 presents, we will have
    // reallocated all our buffers, and we will have done so in a manner that's much less
    // likely to produce delays or glitches.
    constexpr UINT numberOfBuffers = 10;
    for (UINT bufferIndex = 0; bufferIndex < numberOfBuffers; bufferIndex++)
    {
        // Advance our present time 1/10th of a second in the future.
        presentTime.value += 1'000'000;

        // Release the old texture/presentation buffer at the presented index.
        auto& replacedTexture = textures[bufferIndex];
        auto& replacedPresentationBuffer = presentationBuffers[bufferIndex];
        replacedTexture.reset();
        replacedPresentationBuffer.reset();

        // Create a new texture/presentation buffer in its place.
        AddNewPresentationBuffer(
            pD3D11Device,
            pPresentationManager,
            200, // Buffer width
            200, // Buffer height
            &replacedTexture,
            &replacedPresentationBuffer);

        // Draw red to the new texture.
        DrawColorToSurface(
            pD3D11Device,
            replacedTexture,
            1.0f, // red
            0.0f, // green
            0.0f); // blue

        // Bind the presentation buffer to the presentation surface.
        pPresentationSurface->SetBuffer(replacedPresentationBuffer.get());

        // Present at the targeted time.
        pPresentationManager->SetTargetTime(presentTime);
        HRESULT hrPresent = pPresentationManager->Present();
        if (hrPresent == PRESENTATION_ERROR_LOST)
        {
            // Our presentation manager has been lost. Return 'false' to the caller to indicate that
            // the presentation manager should be recreated.
            return false;
        }
        else
        {
            FAIL_FAST_IF_FAILED(hrPresent);
        }
    }

    return true;
}
```

## <a name="example-16mdashreading-and-processing-present-statistics"></a>Пример 16. &mdash; чтение и обработка текущей статистики

API сообщает о статистике для каждого переданного объекта. На высоком уровне представленная статистика представляет собой механизм обратной связи, который описывает, как конкретная система была обработана или показана системой. Существует несколько типов статистических данных, которые приложение может зарегистрировать для получения, а инфраструктура статистики в самом API должна быть расширяемой, поэтому в будущем можно добавить дополнительные типы статистики. Этот API описывает, как считывать статистику, а также описывает типы статистических данных, определенные сегодня, и сведения, которые они передают на высоком уровне.

### <a name="c-example"></a>Пример C++

```cpp
// This is an identifier we'll assign to our presentation surface that will be used to reference that
// presentation surface in statistics. This is to avoid referring to a presentation surface by pointer
// in a statistics structure, which has unclear refcounting and lifetime semantics.
static constexpr UINT_PTR myPresentedContentTag = 12345;

bool StatisticsExample(
    _In_ ID3D11Device* pD3D11Device,
    _In_ IPresentationManager* pPresentationManager,
    _In_ IPresentationSurface* pPresentationSurface,
    _In_ vector<com_ptr_failfast<ID3D11Texture2D>>& textures,
    _In_ vector<com_ptr_failfast<IPresentationBuffer>>& presentationBuffers)
{
    // Track a time we'll be presenting to below. Default to the current time, then increment by
    // 1/10th of a second every present.
    SystemInterruptTime presentTime;
    QueryInterruptTimePrecise(&presentTime.value);

    // Register to receive 3 types of statistics.
    FAIL_FAST_IF_FAILED(pPresentationManager->EnablePresentStatisticsKind(
        PresentStatisticsKind_CompositionFrame,
        true));
    FAIL_FAST_IF_FAILED(pPresentationManager->EnablePresentStatisticsKind(
        PresentStatisticsKind_PresentStatus,
        true));
    FAIL_FAST_IF_FAILED(pPresentationManager->EnablePresentStatisticsKind(
        PresentStatisticsKind_IndependentFlipFrame,
        true));

    // Stats come back referencing specific presentation surfaces. We assign 'tags' to presentation
    // surfaces in the API that statistics will use to reference the presentation surface in a
    // statistic.
    pPresentationSurface->SetTag(myPresentedContentTag);

    // Build an array of events that we can wait on.
    vector<unique_event> waitEvents;

    // The lost event will be the first event in our list. This is an event that signifies that
    // something went wrong in the system (due to extreme conditions like memory pressure, or
    // driver issues) that indicate that the presentation manager has been lost, and should no
    // longer be used, and instead should be recreated.
    unique_event lostEvent;
    FAIL_FAST_IF_FAILED(pPresentationManager->GetLostEvent(&lostEvent));
    waitEvents.emplace_back(std::move(lostEvent));

    // The statistics event will be the second event in our list. This event will be signaled
    // by the presentation manager when there are statistics to read back.
    unique_event statisticsEvent;
    FAIL_FAST_IF_FAILED(pPresentationManager->GetPresentStatisticsAvailableEvent(&statisticsEvent));
    waitEvents.emplace_back(std::move(statisticsEvent));

    // Add each buffer's available event to the list of events we will be waiting on.
    for (UINT bufferIndex = 0; bufferIndex < presentationBuffers.size(); bufferIndex++)
    {
        unique_event availableEvent;
        presentationBuffers[bufferIndex]->GetAvailableEvent(&availableEvent);
        waitEvents.emplace_back(std::move(availableEvent));
    }

    // Iterate our workflow 120 times.
    constexpr UINT iterationCount = 120;
    for (UINT i = 0; i < iterationCount; i++)
    {
        // Wait for an event to be signaled.
        DWORD waitResult = WaitForMultipleObjects(
            static_cast<UINT>(waitEvents.size()),
            reinterpret_cast<HANDLE*>(waitEvents.data()),
            FALSE,
            INFINITE);

        // Failfast if the wait hit an error.
        FAIL_FAST_IF((waitResult - WAIT_OBJECT_0) >= waitEvents.size());

        // Our lost event was the first event in the array. If this is signaled, then the caller
        // should recreate the presentation manager. This is very similar to how Direct3D devices
        // can be lost. Assume our caller knows to handle this return value appropriately.
        if (waitResult == WAIT_OBJECT_0)
        {
            return false;
        }

        // The second event in the array is the statistics event. If this event is signaled,
        // read and process our statistics.
        if (waitResult == (WAIT_OBJECT_0 + 1))
        {
            StatisticsExample_ProcessStatistics(pPresentationManager);
        }
        // Otherwise, the event corresponds to a buffer available event that is signaled.
        // Compute the buffer for the available event that was signaled and present a
        // frame.
        else
        {
            DWORD bufferIndex = waitResult - (WAIT_OBJECT_0 + 2);

            // Draw red to the texture.
            DrawColorToSurface(
                pD3D11Device,
                textures[bufferIndex],
                1.0f, // red
                0.0f, // green
                0.0f); // blue

            // Bind the texture to the presentation surface.
            pPresentationSurface->SetBuffer(presentationBuffers[bufferIndex].get());

            // Advance our present time 1/10th of a second in the future.
            presentTime.value += 1'000'000;

            // Present at the targeted time.
            pPresentationManager->SetTargetTime(presentTime);
            HRESULT hrPresent = pPresentationManager->Present();
            if (hrPresent == PRESENTATION_ERROR_LOST)
            {
                // Our presentation manager has been lost. Return 'false' to the caller to indicate that
                // the presentation manager should be recreated.
                return false;
            }
            else
            {
                FAIL_FAST_IF_FAILED(hrPresent);
            }
        }
    }

    return true;
}

void StatisticsExample_ProcessStatistics(
    _In_ IPresentationManager* pPresentationManager)
{
    // Dequeue a single present statistics item. This will return the item
    // and pop it off the queue of statistics.
    com_ptr_failfast<IPresentStatistics> presentStatisticsItem;
    pPresentationManager->GetNextPresentStatistics(&presentStatisticsItem);

    // Read back the present ID this corresponds to.
    UINT64 presentId = presentStatisticsItem->GetPresentId();
    UNREFERENCED_PARAMETER(presentId);

    // Switch on the type of statistic this item corresponds to.
    switch (presentStatisticsItem->GetKind())
    {
        case PresentStatisticsKind_PresentStatus:
        {
            // Present status statistics describe whether a given present was queued for display,
            // skipped due to some future present being a better candidate to display on a given
            // frame, or canceled via the API.
            auto presentStatusStatistics = presentStatisticsItem.query<IPresentStatusStatistics>();

            // Read back the status
            PresentStatus status = presentStatusStatistics->GetPresentStatus();
            UNREFERENCED_PARAMETER(status);

            // Possible values for status:
            //   PresentStatus_Queued
            //   PresentStatus_Skipped
            //   PresentStatus_Canceled;

            // Depending on the status returned, your application can adjust their workflow
            // accordingly. For example, if your application sees that a large percentage of their
            // presents are skipped, it means they are presenting more frames than the system can
            // display. In such a case, your application might decided to lower the rate at which
            // you present frames.
        }
        break;

        case PresentStatisticsKind_CompositionFrame:
        {
            // Composition frame statistics describe how a given present was used in a DWM frame.
            // It includes information such as which monitors displayed the present, whether the
            // present was composed or directly scanned out via an MPO plane, and rendering
            // properties such as what transforms were applied to the rendering. Composition
            // frame statistics are not issued for iflip presents - only for presents issued by the
            // compositor. iflip presents have their own type of statistic (described next).
            auto compositionFrameStatistics =
                presentStatisticsItem.query<ICompositionFramePresentStatistics>();

            // Stats should come back for the present statistics item that we tagged earlier.
            NT_ASSERT(compositionFrameStatistics->GetContentTag() == myPresentedContentTag);

            // The composition frame ID indicates the DWM frame ID that the present was used
            // in.
            CompositionFrameId frameId = compositionFrameStatistics->GetCompositionFrameId();

            // Get the display instance array to indicate which displays showed the present. Each
            // instance of the presentation surface will have an entry in this array. For example,
            // if your application adds the same presentation surface to four different visuals in the
            // visual tree, then each instance in the tree will have an entry in the display instance
            // array. Similarly, if the presentation surface shows up on multiple monitors, then each
            // monitor instance will be accounted for in the display instance array that is
            // returned.
            //
            // Note that the pointer returned from GetDisplayInstanceArray is valid for the
            // lifetime of the ICompositionFramePresentStatistics. Your application must not attempt
            // to read this pointer after the ICompositionFramePresentStatistics has been released
            // to a refcount of 0.
            UINT displayInstanceArrayCount;
            const CompositionFrameDisplayInstance* pDisplayInstances;
            compositionFrameStatistics->GetDisplayInstanceArray(
                &displayInstanceArrayCount,
                &pDisplayInstances);

            for (UINT i = 0; i < displayInstanceArrayCount; i++)
            {
                const auto& displayInstance = pDisplayInstances[i];

                // The following are fields that are available in a display instance.

                // The LUID, VidPnSource, and unique ID of the output and its owning
                // adapter. The unique ID will be bumped when a LUID/VidPnSource is
                // recycled. Applications should use the unique ID to determine when
                // this happens so that they don't try and correlate stats from one
                // monitor with another.
                displayInstance.outputAdapterLUID;
                displayInstance.outputVidPnSourceId;
                displayInstance.outputUniqueId;

                // The instanceKind field indicates how the present was used. It
                // indicates that the present was composed (rendered to DWM's backbuffer),
                // scanned out (via MPO/DFlip) or composed to an intermediate buffer by DWM
                // for effects.
                displayInstance.instanceKind;

                // The finalTransform field indicates the transform at which the present was
                // shown in world space. It will include all ancestor visual transforms and
                // can be used to know how it was rendered in the global visual tree.
                displayInstance.finalTransform;

                // The requiredCrossAdapterCopy field indicates whether or not we needed to
                // copy your application's buffer to a different adapter in order to display
                // it. Applications should use this to determine whether or not they should
                // reallocate their buffers onto a different adapter for better performance.
                displayInstance.requiredCrossAdapterCopy;

                // The colorSpace field indicates the colorSpace of the output that the
                // present was rendered to.
                displayInstance.colorSpace;

                // For example, if your application sees that the finalTransform is scaling your
                // content by 2x, you might elect to pre-render that scale into your presentation
                // surface, and then add a 1/2 scale. At which point, the finalTransform should
                // be 1x, and some MPO hardware will be more likely to MPO a presentation surface
                // with a 1x scale applied, since some hardware has a maximum they are able to
                // scale in an MPO plane. Similarly, if your application's content is being scaled
                // down on screen, you may wish to simply render its content at a
                // smaller scale to conserve resources, and apply an enlargement transform.
            }

            // Additionally, we can use the CompositionFrameId reported by the statistic
            // to query timing-related information about that specific frame via the new
            // composition timing API, such as when that frame showed up on screen.
            // Note this is achieved using a separate API from the composition swapchain API, but
            // using the composition frame ID reported in the composition swapchain API to
            // properly specify which frame your application wants timing information from.
            COMPOSITION_FRAME_TARGET_STATS frameTargetStats;
            COMPOSITION_TARGET_STATS targetStats[4];
            frameTargetStats.targetCount = ARRAYSIZE(targetStats);
            frameTargetStats.targetStats = targetStats;

            // Specify the frameId that we got from stats in order to pass to the call
            // below and retrieve timing information about that frame.
            frameTargetStats.frameId = frameId;
            FAIL_FAST_IF_FAILED(DCompositionGetTargetStatistics(1, &frameTargetStats));

            // If the frameTargetStats comes back with a 0 frameId, it means the frame isn't
            // part of statistics. This might mean that it has expired out of
            // DCompositionGetTargetStatistics history, but that call keeps a history buffer
            // roughly equivalent to ~5 seconds worth of frame history, so if your application
            // is processing statistics from the presentation manager relatively regularly,
            // by all accounts it shouldn't worry about DCompositionGetTargetStatistics
            // history expiring. The more likely scenario when this occurs is that it's too
            // early, and that this frame isn't part of statistics YET. In that case, your application
            // should defer processing for this frame, and try again later. For the purposes
            // if sample brevity, we don't bother trying again here. A good method to use would
            // be to add this present info to a list of presents that we haven't gotten target
            // statistics for yet, and try again for all presents in that list any time we get
            // a new PresentStatisticsKind_CompositionFrame for a future frame.
            if (frameTargetStats.frameId == frameId)
            {
                // The targetCount will represent the count of outputs the given frame
                // applied to.
                frameTargetStats.targetCount;

                // The targetTime corresponds to the wall clock QPC time DWM was
                // targeting for the frame.
                frameTargetStats.targetTime;

                for (UINT i = 0; i < frameTargetStats.targetCount; i++)
                {
                    const auto& targetStat = frameTargetStats.targetStats[i];

                    // The present time corresponds to the targeted present time of the composition
                    // frame.
                    targetStat.presentTime;

                    // The target ID corresponds to the LUID/VidPnSourceId/Unique ID for the given
                    // target.
                    targetStat.targetId;

                    // The completedStats convey information about the time a compositor frame was
                    // completed, which marks the time any of its associated composition swapchain API
                    // presents entered the displayed state. In particular, your application might wish
                    // to use the 'time' to know if a present showed at a time it expected.
                    targetStat.completedStats.presentCount;
                    targetStat.completedStats.refreshCount;
                    targetStat.completedStats.time;

                    // There is various other timing statistics information conveyed by
                    // DCompositionGetTargetStatistics.
                }
            }
        }
        break;

        case PresentStatisticsKind_IndependentFlipFrame:
        {
            // Independent flip frame statistics describe a present that was shown via
            // independent flip.
            auto independentFlipFrameStatistics =
                presentStatisticsItem.query<IIndependentFlipFramePresentStatistics>();

            // Stats should come back for the present statistics item that we tagged earlier.
            NT_ASSERT(independentFlipFrameStatistics->GetContentTag() == myPresentedContentTag);

            // The driver-approved present duration describes the custom present duration that was
            // approved by the driver and applied during the present. This is how, for example, media
            // will know whether or not they got 24hz mode for their content if they requested it.
            independentFlipFrameStatistics->GetPresentDuration();

            // The displayed time is the time the present was confirmed to have been shown
            // on screen.
            independentFlipFrameStatistics->GetDisplayedTime();

            // The adapter LUID/VidpnSource ID describe the output on which the present took
            // place. Unlike the composition statistic above, we don't report a unique ID here
            // because a monitor recycle would kick the presentation out of iflip.
            independentFlipFrameStatistics->GetOutputAdapterLUID();
            independentFlipFrameStatistics->GetOutputVidPnSourceId();
        }
        break;
    }
}
```

## <a name="example-17mdashusing-an-abstraction-layer-to-present-using-either-the-new-composition-swapchain-api-or-dxgi-from-your-application"></a>Пример 17. &mdash; использование слоя абстракции для отображения с помощью нового API-интерфейса композиции имеющуюся цепочку буферов или DXGI из приложения

Учитывая более высокие требования к системе и драйверу нового API-интерфейса имеющуюся цепочку буферов композиции, приложение может использовать DXGI в тех случаях, когда новый API не поддерживается. К счастью, очень просто представить уровень абстракции, который использует любой API, доступный для презентации. В следующем примере показано, как добиться этого.

### <a name="c-example"></a>Пример C++

```cpp
// A base class presentation provider. We'll provide implementations using both DXGI and the new
// composition swapchain API, which the example will use based on what's supported.
class PresentationProvider
{
public:
    virtual void GetBackBuffer(
        _Out_ ID3D11Texture2D** ppBackBuffer) = 0;

    virtual void Present(
        _In_ SystemInterruptTime presentationTime) = 0;

    virtual bool ReadStatistics(
        _Out_ UINT* pPresentCount,
        _Out_ UINT64* pSyncQPCTime) = 0;

    virtual ID3D11Device* GetD3D11DeviceNoRef()
    {
        return m_d3dDevice.get();
    }

protected:
    com_ptr_failfast<ID3D11Device> m_d3dDevice;
};

// An implementation of PresentationProvider using a DXGI swapchain to provide presentation
// functionality.
class DXGIProvider :
    public PresentationProvider
{
public:
    DXGIProvider(
        _In_ UINT width,
        _In_ UINT height,
        _In_ UINT bufferCount)
    {
        com_ptr_failfast<IDXGIAdapter> dxgiAdapter;
        com_ptr_failfast<IDXGIFactory7> dxgiFactory;
        com_ptr_failfast<IDXGISwapChain1> dxgiSwapchain;
        com_ptr_failfast<ID3D11DeviceContext> d3dDeviceContext;

        // Direct3D device creation flags.
        UINT deviceCreationFlags =
            D3D11_CREATE_DEVICE_BGRA_SUPPORT |
            D3D11_CREATE_DEVICE_SINGLETHREADED;

        // Create the Direct3D device.
        FAIL_FAST_IF_FAILED(D3D11CreateDevice(
            nullptr,                   // No adapter
            D3D_DRIVER_TYPE_HARDWARE,  // Hardware device
            nullptr,                   // No module
            deviceCreationFlags,       // Device creation flags
            nullptr, 0,                // Highest available feature level
            D3D11_SDK_VERSION,         // API version
            &m_d3dDevice,              // Resulting interface pointer
            nullptr,                   // Actual feature level
            &d3dDeviceContext));       // Device context

        // Make our way from the Direct3D device to the DXGI factory.
        auto dxgiDevice = m_d3dDevice.query<IDXGIDevice>();
        FAIL_FAST_IF_FAILED(dxgiDevice->GetParent(IID_PPV_ARGS(&dxgiAdapter)));
        FAIL_FAST_IF_FAILED(dxgiAdapter->GetParent(IID_PPV_ARGS(&dxgiFactory)));

        // Create a swapchain matching the desired parameters.
        DXGI_SWAP_CHAIN_DESC1 desc = {};
        desc.Width = width;
        desc.Height = height;
        desc.Format = DXGI_FORMAT_B8G8R8A8_UNORM;
        desc.BufferUsage = DXGI_USAGE_RENDER_TARGET_OUTPUT;
        desc.SampleDesc.Count = 1;
        desc.SampleDesc.Quality = 0;
        desc.BufferCount = bufferCount;
        desc.Scaling = DXGI_SCALING_STRETCH;
        desc.SwapEffect = DXGI_SWAP_EFFECT_FLIP_SEQUENTIAL;
        desc.AlphaMode = DXGI_ALPHA_MODE_PREMULTIPLIED;
        FAIL_FAST_IF_FAILED(dxgiFactory->CreateSwapChainForComposition(
            m_d3dDevice.get(),
            &desc,
            nullptr,
            &dxgiSwapchain));

        // Store the swapchain.
        dxgiSwapchain.query_to(&m_swapchain);
    }

    void GetBackBuffer(
        _Out_ ID3D11Texture2D** ppBackBuffer) override
    {
        // Get the backbuffer directly from the swapchain.
        FAIL_FAST_IF_FAILED(m_swapchain->GetBuffer(
            m_swapchain->GetCurrentBackBufferIndex(),
            IID_PPV_ARGS(ppBackBuffer)));
    }

    void Present(
        _In_ SystemInterruptTime presentationTime) override
    {
        // Convert the passed presentation time to a present interval. The implementation is
        // not provided here, as there's a great deal of complexity around computing this
        // most accurately, but it essentially boils down to taking the time from now and
        // figuring out the number of vblanks that corresponds to that time duration.
        UINT vblankIntervals = ComputePresentIntervalFromTime(presentationTime);

        // Issue a present to the swapchain. If we wanted to allow for a time to be specified,
        // code here could convert the time to a present duration, which could be passed here.
        FAIL_FAST_IF_FAILED(m_swapchain->Present(vblankIntervals, 0));
    }

    bool ReadStatistics(
        _Out_ UINT* pPresentCount,
        _Out_ UINT64* pSyncQPCTime) override
    {
        // Zero our output parameters initially.
        *pPresentCount = 0;
        *pSyncQPCTime = 0;

        // Grab frame statistics from the swapchain.
        DXGI_FRAME_STATISTICS frameStatistics;
        FAIL_FAST_IF_FAILED(m_swapchain->GetFrameStatistics(&frameStatistics));

        // If the statistics have changed since our last read, then return the new information
        // to the caller.
        bool hasNewStats = false;
        if (frameStatistics.PresentCount > m_lastPresentCount)
        {
            m_lastPresentCount = frameStatistics.PresentCount;
            hasNewStats = true;
            *pPresentCount = frameStatistics.PresentCount;
            *pSyncQPCTime = frameStatistics.SyncQPCTime.QuadPart;
        }

        return hasNewStats;
    }

private:
    com_ptr_failfast<IDXGISwapChain4> m_swapchain;
    UINT m_lastPresentCount = 0;
};

// An implementation of PresentationProvider using the composition swapchain API to provide
// presentation functionality.
class PresentationAPIProvider :
    public PresentationProvider
{
public:
    PresentationAPIProvider(
        _In_ UINT width,
        _In_ UINT height,
        _In_ UINT bufferCount)
    {
        // Create the presentation manager and presentation surface using the function defined in a
        // previous example.
        MakePresentationManagerAndPresentationSurface(
            &m_d3dDevice,
            &m_presentationManager,
            &m_presentationSurface,
            m_presentationSurfaceHandle);

        // Register for present statistics.
        FAIL_FAST_IF_FAILED(m_presentationManager->EnablePresentStatisticsKind(
            PresentStatisticsKind_CompositionFrame,
            true));

        // Get the statistics event from the presentation manager.
        FAIL_FAST_IF_FAILED(m_presentationManager->GetPresentStatisticsAvailableEvent(
            &m_statisticsAvailableEvent));

        // Create and register the specified number of presentation buffers.
        for (UINT i = 0; i < bufferCount; i++)
        {
            com_ptr_failfast<ID3D11Texture2D> texture;
            com_ptr_failfast<IPresentationBuffer> presentationBuffer;
            AddNewPresentationBuffer(
                m_d3dDevice.get(),
                m_presentationManager.get(),
                width,
                height,
                &texture,
                &presentationBuffer);

            // Add the new presentation buffer and texture to our array.
            m_textures.push_back(texture);
            m_presentationBuffers.push_back(presentationBuffer);

            // Store the available event for the presentation buffer.
            unique_event availableEvent;
            FAIL_FAST_IF_FAILED(presentationBuffer->GetAvailableEvent(&availableEvent));
            m_bufferAvailableEvents.emplace_back(std::move(availableEvent));
        }
    }

    void GetBackBuffer(
        _Out_ ID3D11Texture2D** ppBackBuffer) override
    {
        // Query an available backbuffer using our available events.
        DWORD waitIndex = WaitForMultipleObjects(
            static_cast<UINT>(m_bufferAvailableEvents.size()),
            reinterpret_cast<HANDLE*>(m_bufferAvailableEvents.data()),
            FALSE,
            INFINITE);
        UINT bufferIndex = waitIndex - WAIT_OBJECT_0;

        // Set the backbuffer to be the next presentation buffer.
        FAIL_FAST_IF_FAILED(m_presentationSurface->SetBuffer(m_presentationBuffers[bufferIndex].get()));

        // Return the backbuffer to the caller.
        m_textures[bufferIndex].query_to(ppBackBuffer);
    }

    void Present(
        _In_ SystemInterruptTime presentationTime) override
    {
        // Present at the targeted time.
        m_presentationManager->SetTargetTime(presentationTime);
        HRESULT hrPresent = m_presentationManager->Present();
        if (hrPresent == PRESENTATION_ERROR_LOST)
        {
            // Our presentation manager has been lost. See previous examples regarding how to handle this.
            return;
        }
        else
        {
            FAIL_FAST_IF_FAILED(hrPresent);
        }
    }

    bool ReadStatistics(
        _Out_ UINT* pPresentCount,
        _Out_ UINT64* pSyncQPCTime) override
    {
        // Zero our out parameters initially.
        *pPresentCount = 0;
        *pSyncQPCTime = 0;

        bool hasNewStats = false;

        // Peek at the statistics available event state to see if we've got new statistics.
        while (WaitForSingleObject(m_statisticsAvailableEvent.get(), 0) == WAIT_OBJECT_0)
        {
            // Pop a statistics item to process.
            com_ptr_failfast<IPresentStatistics> statisticsItem;
            FAIL_FAST_IF_FAILED(m_presentationManager->GetNextPresentStatistics(
                &statisticsItem));

            // If this is a composition frame stat, process it.
            if (statisticsItem->GetKind() == PresentStatisticsKind_CompositionFrame)
            {
                // We've got new stats to report.
                hasNewStats = true;

                // Convert to composition frame statistic item.
                auto frameStatisticsItem = statisticsItem.query<ICompositionFramePresentStatistics>();

                // Query DirectComposition's target statistics API to determine the completed time.
                COMPOSITION_FRAME_TARGET_STATS frameTargetStats;
                COMPOSITION_TARGET_STATS targetStats[4];
                frameTargetStats.targetCount = ARRAYSIZE(targetStats);
                frameTargetStats.targetStats = targetStats;
                // Specify the frameId we got from stats in order to pass to the call
                // below and retrieve timing information about that frame.
                frameTargetStats.frameId = frameStatisticsItem->GetCompositionFrameId();
                FAIL_FAST_IF_FAILED(DCompositionGetTargetStatistics(1, &frameTargetStats));

                // Return the statistics information for the first target.
                *pPresentCount = static_cast<UINT>(frameStatisticsItem->GetPresentId());
                *pSyncQPCTime = frameTargetStats.targetStats[0].completedStats.time;

                // Note that there's a much richer variety of statistics information in the new
                // API that can be used to infer much more than is possible with DXGI frame
                // statistics.
            }
        }

        return hasNewStats;
    }

    static bool IsSupportedOnSystem()
    {
        // Direct3D device creation flags. The composition swapchain API requires that applications disable internal
        // driver threading optimizations, as these optimizations break synchronization of the API.
        // If this flag isn't present, then the API will fail the call to create the presentation factory.
        UINT deviceCreationFlags =
            D3D11_CREATE_DEVICE_BGRA_SUPPORT |
            D3D11_CREATE_DEVICE_SINGLETHREADED |
            D3D11_CREATE_DEVICE_PREVENT_INTERNAL_THREADING_OPTIMIZATIONS;

        // Create the Direct3D device.
        com_ptr_failfast<ID3D11Device> d3dDevice;
        com_ptr_failfast<ID3D11DeviceContext> d3dDeviceContext;
        FAIL_FAST_IF_FAILED(D3D11CreateDevice(
            nullptr,                   // No adapter
            D3D_DRIVER_TYPE_HARDWARE,  // Hardware device
            nullptr,                   // No module
            deviceCreationFlags,       // Device creation flags
            nullptr, 0,                // Highest available feature level
            D3D11_SDK_VERSION,         // API version
            &d3dDevice,                // Resulting interface pointer
            nullptr,                   // Actual feature level
            &d3dDeviceContext));       // Device context

        // Call the composition swapchain API export to create the presentation factory.
        com_ptr_failfast<IPresentationFactory> presentationFactory;
        FAIL_FAST_IF_FAILED(CreatePresentationFactory(
            d3dDevice.get(),
            IID_PPV_ARGS(&presentationFactory)));

        // Now determine whether the system is capable of supporting the composition swapchain API based
        // on the capability that's reported by the presentation factory.
        return presentationFactory->IsPresentationSupported();
    }

private:
    com_ptr_failfast<IPresentationManager> m_presentationManager;
    com_ptr_failfast<IPresentationSurface> m_presentationSurface;
    vector<com_ptr_failfast<ID3D11Texture2D>> m_textures;
    vector<com_ptr_failfast<IPresentationBuffer>> m_presentationBuffers;
    vector<unique_event> m_bufferAvailableEvents;
    unique_handle m_presentationSurfaceHandle;
    unique_event m_statisticsAvailableEvent;
};

void DXGIOrPresentationAPIExample()
{
    // Get the current system time. We'll base our 'PresentAt' time on this result.
    SystemInterruptTime currentTime;
    QueryInterruptTimePrecise(&currentTime.value);

    // Track a time we'll be presenting at below. Default to the current time, then increment by
    // 1/10th of a second every present.
    auto presentTime = currentTime;

    // Allocate a presentation provider using the composition swapchain API if it is supported;
    // otherwise fall back to DXGI.
    unique_ptr<PresentationProvider> presentationProvider;
    if (PresentationAPIProvider::IsSupportedOnSystem())
    {
        presentationProvider = std::make_unique<PresentationAPIProvider>(
            500, // Buffer width
            500, // Buffer height
            6);  // Number of buffers
    }
    else
    {
        // System doesn't support the composition swapchain API. Fall back to DXGI.
        presentationProvider = std::make_unique<DXGIProvider>(
            500, // Buffer width
            500, // Buffer height
            6);  // Number of buffers
    }

    // Present 50 times.
    constexpr UINT numPresents = 50;
    for (UINT i = 0; i < 50; i++)
    {
        // Advance our present time 1/10th of a second in the future.
        presentTime.value += 1'000'000;

        // Call the presentation provider to get a backbuffer to render to.
        com_ptr_failfast<ID3D11Texture2D> backBuffer;
        presentationProvider->GetBackBuffer(&backBuffer);

        // Render to the backbuffer.
        DrawColorToSurface(
            presentationProvider->GetD3D11DeviceNoRef(),
            backBuffer,
            1.0f, // red
            0.0f, // green
            0.0f); // blue

        // Present the backbuffer.
        presentationProvider->Present(presentTime);

        // Process statistics.
        bool hasNewStats;
        UINT64 presentTime;
        UINT presentCount;
        hasNewStats = presentationProvider->ReadStatistics(
            &presentCount,
            &presentTime);
        if (hasNewStats)
        {
            // Process these statistics however your application wishes.
        }
    }
}
```

## <a name="related-topics"></a>Связанные темы

* [Имеющуюся цепочку буферов композиции](comp-swapchain-portal.md)
