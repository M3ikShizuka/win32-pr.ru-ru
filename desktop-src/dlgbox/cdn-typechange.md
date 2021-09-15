---
title: Код уведомления CDN_TYPECHANGE (Коммдлг. h)
description: Отправляется в стиле обозревателя в диалоговом окне Открыть или сохранить как, когда пользователь выбирает новый тип файла в поле со списком типы файлов.
ms.assetid: fb8324db-e435-4ef2-aac5-506a6b7adb2c
keywords:
- CDN_TYPECHANGE диалоговых окон кода уведомления
topic_type:
- apiref
api_name:
- CDN_TYPECHANGE
api_location:
- Commdlg.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3922dd71b70ace579fa4b5f2318776779afdfa4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127566566"
---
# <a name="cdn_typechange-notification-code"></a>CDN \_ Код уведомления ТИПЕЧАНЖЕ

\[начиная с Windows Vista общие диалоговые окна " **открыть** " и " **сохранить как** " были заменены [диалоговым окном общих элементов](../shell/common-file-dialog.md). Рекомендуется использовать API-интерфейс общего элемента, а не эти диалоговые окна из библиотеки общих диалоговых окон.\]

Отправляется в стиле обозревателя в диалоговом окне **Открыть** или **Сохранить как** , когда пользователь выбирает новый тип файла в поле со списком типы файлов.

Процедура обработчика [*офнхукпрок*](/windows/win32/api/commdlg/nc-commdlg-lpofnhookproc) получает это сообщение в виде сообщения [**WM \_ Notify**](../controls/wm-notify.md) .


```C++
#define CDN_FIRST               (0U-601U)
#define CDN_TYPECHANGE          (CDN_FIRST - 0x0006)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Этот параметр не используется.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**офнотифи**](/windows/desktop/api/Commdlg/ns-commdlg-ofnotifya) .

структура [**офнотифи**](/windows/desktop/api/Commdlg/ns-commdlg-ofnotifya) содержит структуру [**NMHDR**](/windows/win32/api/richedit/ns-richedit-nmhdr) , элемент **кода** которой указывает на сообщение уведомления о **CDN \_ типечанже** .

Структура [**офнотифи**](/windows/desktop/api/Commdlg/ns-commdlg-ofnotifya) также содержит указатель на структуру [**OpenFileName**](/windows/win32/api/commdlg/ns-commdlg-openfilenamea) , член **нфилтериндекс** которой указывает индекс только что выбранного фильтра типа файла.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Это сообщение не имеет возвращаемого значения.

## <a name="remarks"></a>Remarks

Система отправляет это уведомление только в том случае, если диалоговое окно было создано с помощью значения **\_ обозревателя ОФН** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                               |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                     |
| Заголовок<br/>                   | <dl> <dt>коммдлг. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Ссылки**
</dt> <dt>

[**GetOpenFileName**](/windows/desktop/api/Commdlg/nf-commdlg-getopenfilenamea)
</dt> <dt>

[**жетсавефиленаме**](/windows/desktop/api/Commdlg/nf-commdlg-getsavefilenamea)
</dt> <dt>

[*офнхукпрок*](/windows/win32/api/commdlg/nc-commdlg-lpofnhookproc)
</dt> <dt>

[**офнотифи**](/windows/desktop/api/Commdlg/ns-commdlg-ofnotifya)
</dt> <dt>

[**OPENFILENAME**](/windows/win32/api/commdlg/ns-commdlg-openfilenamea)
</dt> <dt>

**Основные понятия**
</dt> <dt>

[Библиотека общих диалоговых окон](common-dialog-box-library.md)
</dt> </dl>

