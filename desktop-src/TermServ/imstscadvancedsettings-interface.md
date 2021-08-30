---
title: Интерфейс Имстскадванцедсеттингс
description: Содержит методы для получения и задания свойств, обеспечивающих кэширование растровых изображений, сжатие, а также перенаправление принтера и буфера обмена.
ms.assetid: 3385e843-be05-4801-8d59-6395d95686b1
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов интерфейса Имстскадванцедсеттингс
- Службы удаленных рабочих столов интерфейса Имстскадванцедсеттингс, описание
topic_type:
- apiref
api_name:
- IMsTscAdvancedSettings
api_location:
- MsTscAx.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: edc379375456feb5de50abdc68ff2cc2da463fbe
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122475350"
---
# <a name="imstscadvancedsettings-interface"></a>Интерфейс Имстскадванцедсеттингс

Содержит методы для получения и задания свойств, обеспечивающих кэширование растровых изображений, сжатие, а также перенаправление принтера и буфера обмена. Можно также указать имена клиентских библиотек DLL для виртуальных каналов.

Экземпляр этого интерфейса можно получить с помощью свойства [**имстскакс:: адванцедсеттингс**](imstscax-advancedsettings.md) .

## <a name="members"></a>Элементы

Интерфейс **имстскадванцедсеттингс** наследует от интерфейса [**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch) . **Имстскадванцедсеттингс** также имеет следующие типы членов:

-   [Свойства](#properties)

### <a name="properties"></a>Элемент Property

Интерфейс **имстскадванцедсеттингс** имеет следующие свойства.




| Свойство | Тип доступа | Описание | 
|----------|-------------|-------------|
| <a href="imstscadvancedsettings-allowbackgroundinput.md"><strong>алловбаккграундинпут</strong></a><br /> | Чтение/запись<br /> | Указывает, включен ли режим фонового ввода.<br /> | 
| <a href="imstscadvancedsettings-bitmapperistence.md"><strong>битмапперистенце</strong></a><br /> | Чтение/запись<br /> | Указывает, включено ли кэширование растровых изображений.<br /><blockquote>[!Note]<br />Орфографическая ошибка в имени свойства находится в выпущенной версии элемента управления.</blockquote><br /> | 
| <a href="imstscadvancedsettings-compress.md"><strong>Повторно</strong></a><br /> | Чтение/запись<br /> | Указывает, включено ли сжатие.<br /> | 
| <a href="imstscadvancedsettings-containerhandledfullscreen.md"><strong>контаинерхандледфуллскрин</strong></a><br /> | Чтение/запись<br /> | Указывает, включен ли полноэкранный режим, обрабатываемый контейнером.<br /> | 
| <a href="imstscadvancedsettings-disablerdpdr.md"><strong>дисаблердпдр</strong></a><br /> | Чтение/запись<br /> | Указывает, включено ли перенаправление принтеров и буферов обмена.<br /> | 
| <a href="imstscadvancedsettings-iconfile.md"><strong>иконфиле</strong></a><br /> | Только на запись<br /> | Указывает имя файла, содержащего данные значков, которые будут доступны при отображении клиента в полноэкранном режиме.<br /> | 
| <a href="imstscadvancedsettings-iconindex.md"><strong>икониндекс</strong></a><br /> | Только на запись<br /> | Задает индекс значка в текущем файле значка.<br /> | 
| <a href="imstscadvancedsettings-keyboardlayoutstr.md"><strong>кэйбоардлайаутстр</strong></a><br /> | Только на запись<br /> | Задает имя активного идентификатора языка ввода (прежнее название раскладки клавиатуры), используемого для соединения.<br /> | 
| <a href="imstscadvancedsettings-plugindlls.md"><strong>плугиндллс</strong></a><br /> | Только на запись<br /> | Указывает имена клиентских DLL-библиотек виртуальных каналов для загрузки.<br /> | 




 

## <a name="remarks"></a>Комментарии

Этот интерфейс расширен следующими интерфейсами, при этом каждый новый интерфейс наследует все методы и свойства предыдущих интерфейсов:

-   [**имсрдпклиентадванцедсеттингс**](imsrdpclientadvancedsettings-interface.md)
-   [**IMsRdpClientAdvancedSettings2**](imsrdpclientadvancedsettings2.md)
-   [**IMsRdpClientAdvancedSettings3**](imsrdpclientadvancedsettings3.md)
-   [**IMsRdpClientAdvancedSettings4**](imsrdpclientadvancedsettings4.md)
-   [**IMsRdpClientAdvancedSettings5**](imsrdpclientadvancedsettings5.md)
-   [**IMsRdpClientAdvancedSettings6**](imsrdpclientadvancedsettings6.md)
-   [**IMsRdpClientAdvancedSettings7**](imsrdpclientadvancedsettings7.md)

Дополнительные сведения о веб-подключение к удаленному рабочему столу см. в разделе [требования для веб-подключение к удаленному рабочему столу](requirements-for-remote-desktop-web-connection.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                  |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                            |
| Библиотека типов<br/>             | <dl> <dt>MsTscAx.dll</dt> </dl>    |
| DLL<br/>                      | <dl> <dt>MsTscAx.dll</dt> </dl>    |
| IID<br/>                      | IID \_ имстскадванцедсеттингс определен как 809945cc-4b3b-4a92-a6b0-dbf9b5f2ef2d<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**IDispatch**](/windows/win32/api/oaidl/nn-oaidl-idispatch)
</dt> <dt>

[Справочник по веб-подключение к удаленному рабочему столу](remote-desktop-web-connection-reference.md)
</dt> </dl>

 

