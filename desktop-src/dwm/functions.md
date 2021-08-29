---
title: Функции DWM
description: В этом разделе содержатся сведения о функциях диспетчер окон рабочего стола (DWM).
ms.assetid: 525807fe-c5d7-4997-87b9-a14d02c33cc3
keywords:
- Диспетчер окон рабочего стола (DWM), справочные материалы
- DWM (диспетчер окон рабочего стола), Справочник
- Диспетчер окон рабочего стола (DWM), функции
- DWM (диспетчер окон рабочего стола), функции
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: dd25ecbea1f7e08d8a7d5832d01908fc088e9be2
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122482310"
---
# <a name="dwm-functions"></a>Функции DWM

В этом разделе содержатся сведения о функциях диспетчер окон рабочего стола (DWM).

## <a name="in-this-section"></a>В этом разделе




| Раздел | Описание | 
|-------|-------------|
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmattachmilcontent"><strong>двматтачмилконтент</strong></a><br /> | Эта функция не реализована.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmdefwindowproc"><strong>двмдефвиндовпрок</strong></a><br /> | Процедура окна по умолчанию для проверки попадания DWM в области, не являющейся клиентской.<br /> Также необходимо убедиться, что для <a href="/windows/desktop/inputdev/wm-ncmouseleave"><strong>WM_NCMOUSELEAVE</strong></a> сообщения вызывается метод <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmdefwindowproc"><strong>двмдефвиндовпрок</strong></a> . Если <strong>двмдефвиндовпрок</strong> не вызывается для сообщения <strong>WM_NCMOUSELEAVE</strong> , DWM не удаляет выделение из кнопок <strong>развертывания</strong>, <strong>сворачивания</strong>и <strong>закрытия</strong> , когда курсор покидает окно.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmdetachmilcontent"><strong>двмдетачмилконтент</strong></a><br /> | Эта функция не реализована.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmenableblurbehindwindow"><strong>DwmEnableBlurBehindWindow</strong></a><br /> | Включает эффект размытия для указанного окна.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmenablecomposition"><strong>двменаблекомпоситион</strong></a><br /> | Включает или отключает композицию DWM. <br /><blockquote>[!Note]<br />Эта функция является устаревшей по отношению к Windows 8. Диспетчер DWM больше не может быть отключен программным способом.</blockquote><br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmenablemmcss"><strong>двменаблеммксс</strong></a><br /> | Уведомляет DWM о необходимости отказаться от планирования службы обработки отказов (MMCSS) класса мультимедиа, пока вызывающий процесс активен.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmextendframeintoclientarea"><strong>DwmExtendFrameIntoClientArea</strong></a><br /> | Расширяет рамку окна в клиентскую область.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmflush"><strong>двмфлуш</strong></a><br /> | Выдает вызов сброса, который блокирует вызывающий объект до следующего присутствия, когда все обновления Microsoft DirectX Surface, которые в настоящее время были выполнены. Это компенсирует очень сложный монтажный кадр или вызов процессов с очень низким приоритетом.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgetcolorizationcolor"><strong>двмжетколоризатионколор</strong></a><br /> | Извлекает текущий цвет, используемый для композиции DWM с эффектом стекла. Это значение основано на текущей цветовой схеме и может быть изменено пользователем. Приложения могут прослушивать изменения цвета, обрабатывая уведомление <a href="wm-dwmcolorizationcolorchanged.md"><strong>WM_DWMCOLORIZATIONCOLORCHANGED</strong></a> .<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgetcompositiontiminginfo"><strong>двмжеткомпоситионтимингинфо</strong></a><br /> | Извлекает сведения о текущем времени композиции для указанного окна.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgetgraphicsstreamclient"><strong>двмжетграфиксстреамклиент</strong></a><br /> | Эта функция не реализована.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgetgraphicsstreamtransformhint"><strong>двмжетграфиксстреамтрансформхинт</strong></a><br /> | Эта функция не реализована.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgettransportattributes"><strong>двмжеттранспортаттрибутес</strong></a><br /> | Получает атрибуты транспорта.<br /> | 
| <a href="/windows/desktop/api/dwmapi/nf-dwmapi-dwmgetunmettabrequirements"><strong>двмжетунметтабрекуирементс</strong></a><br /> | <blockquote><strong>Примечание</strong> .  эта функция является общедоступной, но нефункциональной для Windows 10 версии 1803.</blockquote>Проверяет требования, необходимые для получения вкладок в строке заголовка приложения для указанного окна.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmgetwindowattribute"><strong>двмжетвиндоваттрибуте</strong></a><br /> | Извлекает текущее значение указанного атрибута, примененного к окну.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwminvalidateiconicbitmaps"><strong>двминвалидатеиконикбитмапс</strong></a><br /> | Вызывается приложением для указания того, что все ранее предоставленные точечные рисунки из окна, как эскизы, так и Просмотр представлений, должны быть обновлены.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmiscompositionenabled"><strong>DwmIsCompositionEnabled</strong></a><br /> | Получает значение, указывающее, включена ли композиция DWM. приложения на компьютерах с Windows 7 и более ранних версий могут прослушивать изменения состояния композиции, обрабатывая уведомление <a href="wm-dwmcompositionchanged.md"><strong>WM_DWMCOMPOSITIONCHANGED</strong></a> .<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmmodifypreviousdxframeduration"><strong>двммодифипревиаусдксфрамедуратион</strong></a><br /> | Изменяет число обновлений монитора, с помощью которых будет отображаться предыдущий кадр. <br /><a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmmodifypreviousdxframeduration"><strong>Двммодифипревиаусдксфрамедуратион</strong></a> больше не поддерживается. начиная с Windows 8.1, вызовы метода <strong>двммодифипревиаусдксфрамедуратион</strong> всегда возвращают E_NOTIMPL.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmquerythumbnailsourcesize"><strong>двмкуерисумбнаилсаурцесизе</strong></a><br /> | Получает исходный размер эскиза DWM.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmregisterthumbnail"><strong>DwmRegisterThumbnail</strong></a><br /> | Создает отношение эскиза DWM между конечным и исходным окнами.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmrendergesture"><strong>двмрендержестуре</strong></a><br /> | Уведомляет DWM о том, что Контактное лицо было распознано как жест, и что DWM должен нарисовать отзыв для этого жеста.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmsetdxframeduration"><strong>двмсетдксфрамедуратион</strong></a><br /> | Задает число обновлений монитора, по которым отображается отображаемый кадр. <br /><a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmsetdxframeduration"><strong>Двмсетдксфрамедуратион</strong></a> больше не поддерживается. начиная с Windows 8.1, вызовы метода <strong>двмсетдксфрамедуратион</strong> всегда возвращают E_NOTIMPL.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmseticoniclivepreviewbitmap"><strong>двмсетиконикливепревиевбитмап</strong></a><br /> | Задает статический точечный рисунок для отображения <em>динамического предварительного просмотра</em> (также известного как <em>Предварительный просмотр</em>) окна или вкладки. Панель задач может использовать это растровое изображение, чтобы отобразить полный предварительный просмотр окна или вкладки.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmseticonicthumbnail"><strong>двмсетикониксумбнаил</strong></a><br /> | Задает статический точечный рисунок на окне или вкладке для использования в качестве эскиза. Панель задач может использовать это растровое изображение в качестве цели переключателя эскиза для окна или вкладки.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmsetpresentparameters"><strong>двмсетпресентпараметерс</strong></a><br /> | Задает существующие параметры для компоновки кадра. <br /><a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmsetpresentparameters"><strong>Двмсетпресентпараметерс</strong></a> больше не поддерживается. начиная с Windows 8.1, вызовы метода <strong>двмсетпресентпараметерс</strong> всегда возвращают E_NOTIMPL.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmsetwindowattribute"><strong>двмсетвиндоваттрибуте</strong></a><br /> | Задает значение для атрибутов окна, не являющихся клиентским рендерингом.<br /> | 
| <a href="/windows/desktop/api/dwmapi/nf-dwmapi-dwmshowcontact"><strong>двмшовконтакт</strong></a><br /> | Вызывается приложением или платформой для указания типа визуальной обратной связи для отображения в ответ на конкретный контакт или связь с пером.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmtethercontact"><strong>двмтесерконтакт</strong></a><br /> | Позволяет выполнять графический отзыв о сенсорном взаимодействии и перетаскивать взаимодействия с пользователем.<br /> | 
| <a href="/windows/desktop/api/dwmapi/nf-dwmapi-dwmtransitionownedwindow"><strong>двмтранситионовнедвиндов</strong></a><br /> | Координирует анимацию окон инструментов с помощью DWM.<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmunregisterthumbnail"><strong>двмунрегистерсумбнаил</strong></a><br /> | Удаляет связь эскиза DWM, созданную функцией <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmregisterthumbnail"><strong>DwmRegisterThumbnail</strong></a> .<br /> | 
| <a href="/windows/desktop/api/Dwmapi/nf-dwmapi-dwmupdatethumbnailproperties"><strong>DwmUpdateThumbnailProperties</strong></a><br /> | Обновляет свойства эскиза DWM.<br /> | 




 

 

