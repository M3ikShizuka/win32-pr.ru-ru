---
title: Пример диалогового окна "Открыть"
description: Пример Shapes, который мы использовали, немного надуманный. давайте перейдем к COM-объекту, который можно использовать в реальной Windows программе открыть диалоговое окно.
ms.assetid: f426cf83-ed24-4eeb-bc28-b5871b824525
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d896c5928c5bcf5e7dae7835d011ddf0f1fbd6e6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127144634"
---
# <a name="example-the-open-dialog-box"></a>Пример. диалоговое окно "Открыть"

`Shapes`Пример, который мы использовали, немного надуманный. давайте вернемся к COM-объекту, который можно использовать в реальной Windows программе: диалоговое окно **открыть** .

![снимок экрана, показывающий диалоговое окно "Открыть"](images/fileopen01.png)

Чтобы отобразить диалоговое окно **Открыть** , программа может использовать COM-объект, называемый объектом диалогового окна общих элементов. В диалоговом окне Общие элементы реализуется интерфейс с именем [**ифилеопендиалог**](/windows/desktop/api/shobjidl_core/nn-shobjidl_core-ifileopendialog), который объявлен в файле заголовка shobjidl. h.

Ниже приведена программа, которая отображает диалоговое окно **Открыть** для пользователя. Если пользователь выбирает файл, программа отображает диалоговое окно, содержащее имя файла.


```C++
#include <windows.h>
#include <shobjidl.h> 

int WINAPI wWinMain(HINSTANCE hInstance, HINSTANCE, PWSTR pCmdLine, int nCmdShow)
{
    HRESULT hr = CoInitializeEx(NULL, COINIT_APARTMENTTHREADED | 
        COINIT_DISABLE_OLE1DDE);
    if (SUCCEEDED(hr))
    {
        IFileOpenDialog *pFileOpen;

        // Create the FileOpenDialog object.
        hr = CoCreateInstance(CLSID_FileOpenDialog, NULL, CLSCTX_ALL, 
                IID_IFileOpenDialog, reinterpret_cast<void**>(&pFileOpen));

        if (SUCCEEDED(hr))
        {
            // Show the Open dialog box.
            hr = pFileOpen->Show(NULL);

            // Get the file name from the dialog box.
            if (SUCCEEDED(hr))
            {
                IShellItem *pItem;
                hr = pFileOpen->GetResult(&pItem);
                if (SUCCEEDED(hr))
                {
                    PWSTR pszFilePath;
                    hr = pItem->GetDisplayName(SIGDN_FILESYSPATH, &pszFilePath);

                    // Display the file name to the user.
                    if (SUCCEEDED(hr))
                    {
                        MessageBoxW(NULL, pszFilePath, L"File Path", MB_OK);
                        CoTaskMemFree(pszFilePath);
                    }
                    pItem->Release();
                }
            }
            pFileOpen->Release();
        }
        CoUninitialize();
    }
    return 0;
}
```



В этом коде используются некоторые понятия, которые будут описаны далее в модуле, поэтому не беспокойтесь, если вы не понимаете все здесь. Ниже приведена базовая структура кода.

1.  Вызов [**CoInitializeEx**](/windows/desktop/api/combaseapi/nf-combaseapi-coinitializeex) для инициализации библиотеки COM.
2.  Вызовите [**CoCreateInstance**](/windows/desktop/api/combaseapi/nf-combaseapi-cocreateinstance) , чтобы создать объект диалогового окна общих элементов и получить указатель на интерфейс [**ифилеопендиалог**](/windows/desktop/api/shobjidl_core/nn-shobjidl_core-ifileopendialog) объекта.
3.  Вызовите метод « **Показать** » объекта, который показывает диалоговое окно для пользователя. Этот метод блокируется до тех пор, пока пользователь не закрывает диалоговое окно.
4.  Вызовите [**метод GetObject объекта.**](/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ifiledialog-getresult) Этот метод возвращает указатель на второй COM-объект, называемый объектом *элемента оболочки* . Элемент оболочки, реализующий интерфейс [**интерфейса IShellItem**](/windows/desktop/api/shobjidl_core/nn-shobjidl_core-ishellitem) , представляет файл, выбранный пользователем.
5.  Вызовите метод « [**выводить**](/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ishellitem-getdisplayname) » элемента оболочки. Этот метод получает путь к файлу в виде строки.
6.  Отображение окна сообщения, в котором отображается путь к файлу.
7.  Вызовите [**CoUninitialize**](/windows/desktop/api/combaseapi/nf-combaseapi-couninitialize) , чтобы отменить инициализацию библиотеки COM.

Шаги 1, 2 и 7 вызывают функции, определяемые библиотекой COM. Это универсальные функции COM. Шаги 3 – 5 вызывают методы, определяемые объектом диалогового окна общих элементов.

В этом примере показаны оба вида создания объектов: универсальная функция [**CoCreateInstance**](/windows/desktop/api/combaseapi/nf-combaseapi-cocreateinstance) и метод ([**result**](/windows/desktop/api/shobjidl_core/nf-shobjidl_core-ifiledialog-getresult)), характерный для объекта диалогового окна общих элементов.

## <a name="next"></a>Следующий

[Управление жизненным циклом объекта](managing-the-lifetime-of-an-object.md)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Открыть образец диалогового окна](open-dialog-box-sample.md)
</dt> </dl>

 

 