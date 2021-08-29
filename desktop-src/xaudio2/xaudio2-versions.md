---
description: XAudio2 — это кросс-платформенный API, который поставляется для использования в Xbox 360, а также версии Windows, включая Windows XP, Windows Vista, Windows 7 и Windows 8.
ms.assetid: 875b44c4-30d6-8a6e-0cfc-9beb8c46f1b4
title: Версии XAudio2
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 8fec5f86ec0ef59898c5ce52dffc8acae37101d0bab384f2537b0d2e23cb6ac5
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119657064"
---
# <a name="xaudio2-versions"></a>Версии XAudio2

XAudio2 — это кросс-платформенный API, который поставляется для использования в Xbox 360, а также версии Windows, включая Windows XP, Windows Vista, Windows 7 и Windows 8. В Xbox 360 XAudio2 поставляется как статическая библиотека, которая компилируется в главный исполняемый файл. в Windows XAudio2 предоставляется в виде библиотеки динамической компоновки (DLL), установленной в системные папки операционной системы.

## <a name="xaudio-29-windows-10-and-redistributable-for-windows-7-and-windows-8x"></a>ксаудио 2,9 (Windows 10 и распространяемый пакет для Windows 7 и Windows 8. x)

XAudio2 версии 2,9 поставляется в составе Windows 10, XAudio2 \_9.DLL вместе с ксаудио 2,8 для поддержки старых приложений. [распространяемая версия ксаудио 2,9](xaudio2-redistributable.md) также доступна для Windows 7 с пакетом обновления 1 (SP1), Windows 8 и Windows 8.1.

Ксаудио 2.9 обновлены со следующими изменениями:

-   Новые флаги создания: \_ модуль отладки XAUDIO2 \_ , \_ подсистема отладчика XAUDIO2 \_ \_ при \_ простое, XAUDIO2 \_ 1024 \_ тактов.
-   Поддержка Ксвма доступна в этой версии XAudio2.
-   функция [**креатехртфапо**](/windows/desktop/api/HrtfApoApi/nf-hrtfapoapi-createhrtfapo) поддерживается в Windows 10 версии ксаудио 2,9.
-   [**XAUDIO2FX \_ \_Параметры ПЕРЕглагола**](/windows/desktop/api/xaudio2fx/ns-xaudio2fx-xaudio2fx_reverb_parameters) теперь включают значение *сидеделай* для систем 7,1.
-   Функция [**ReverbConvertI3DL2ToNative**](/windows/desktop/api/xaudio2fx/nf-xaudio2fx-reverbconverti3dl2tonative) теперь включает параметр логического *севендотонереверб* , включающий переглагол 7,1.

## <a name="xaudio-28-windows-8x"></a>ксаудио 2,8 (Windows 8. x)

XAudio2 версии 2,8 поставляется сегодня как системный компонент в Windows 8, XAudio2 \_8.DLL. Он доступен в папке "Входящие" и не требует повторного распространения с приложением. для разработки Windows 8 для XAudio2 рекомендуется Windows использовать пакет средств разработки программного обеспечения (SDK). Windows SDK для Windows 8 содержит необходимый заголовок и библиотеку импорта для статической компоновки в XAUDIO2 \_8.DLL.

XAudio2 2,8 обновлена со следующими изменениями:

-   эта версия поддерживает Windows разработки приложений для магазина. API XAudio2 можно использовать в приложениях C++/директкс Windows Store.
-   [**XAudio2Create**](/windows/desktop/api/xaudio2/nf-xaudio2-xaudio2create) является неструктурированным вызовом API Win32 и больше не создает CLSID XAudio2. Удалена поддержка создания экземпляра XAudio2 by CoCreateInstance.
-   Функция Initialize теперь неявно вызывается процессом создания и была удалена из интерфейса [**IXAudio2**](/windows/desktop/api/xaudio2/nn-xaudio2-ixaudio2) .
-   Функции перечисления устройств удалены из XAudio2; функции Жетдевицедетаилс и Жетдевицекаунт были удалены из интерфейса [**IXAudio2**](/windows/desktop/api/xaudio2/nn-xaudio2-ixaudio2) . Приложения, которые требуется отобразить на других звуковых устройствах в системе, должны передать строку идентификатора устройства в [**креатемастерингвоице**](/windows/win32/api/xaudio2/nf-xaudio2-ixaudio2-createmasteringvoice) вместо индекса устройства. Устройство подготовки звука по умолчанию можно создать без перечисления.
-   [**IXAudio2MasteringVoice**](/windows/desktop/api/xaudio2/nn-xaudio2-ixaudio2masteringvoice) имеет добавленную функцию [**IXAudio2MasteringVoice:: жетчаннелмаск**](/windows/win32/api/xaudio2/nf-xaudio2-ixaudio2masteringvoice-getchannelmask) для, которая возвращает маску канала для целевого выходного устройства.
-   Библиотеки [X3DAudio](x3daudio.md) и [ксапофкс](xapofx-overview.md) объединяются в XAudio2. Код приложения по-прежнему использует отдельные заголовки, X3DAUDIO. H и КСПОФКС. H, но теперь ссылается на одну библиотеку импорта XAUDIO2 \_ 8. lib.
-   Поддержка Ксвма недоступна в этой версии XAudio2; Ксвма не будет поддерживаться в качестве формата звукового буфера при вызове Креатесаурцевоице. Теперь рекомендуется использовать объект модуля чтения Media Foundation источника для декодирования широкого спектра форматов мультимедиа в буферы PCM в памяти.
-   Теперь [**креатефкс**](/windows/desktop/api/XAPOFX/nf-xapofx-createfx) принимает четыре параметра, а не два. Новые параметры указывают начальные данные в ходе создания [ксапофкс](xapofx-overview.md) .

## <a name="xaudio-27-and-earlier-windows-7"></a>ксаудио 2,7 и более ранних версий (Windows 7)

Все предыдущие версии XAudio2 для использования в приложениях были предоставлены как распространяемые библиотеки DLL в пакете SDK DirectX. Первая версия XAudio2, XAudio2 2,0, поставляется в выпуске пакета SDK DirectX за Март 2008. Последняя версия для поставки пакета SDK DirectX была XAudio2 2,7, которая доступна в последнем выпуске пакета SDK DirectX в июне 2010.

Устаревший пакет SDK DirectX больше не доступен на странице загрузки Майкрософт из-за прекращения использования всего содержимого, подписанного SHA-1. Окончание срока жизни — 2010 июня.

предыдущие версии XAudio2 нельзя использовать для сборки приложений магазина Windows для Windows 8.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Начало работы](getting-started.md)
</dt> <dt>

[Основные понятия XAudio2](xaudio2-key-concepts.md)
</dt> </dl>

[Руководство разработчика по распространяемой версии XAudio 2.9](xaudio2-redistributable.md)
</dt> </dl>
 

 
