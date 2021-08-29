---
title: Сообщение TB_ADDBITMAP (Коммктрл. h)
description: Добавляет одно или несколько изображений в список изображений кнопок, доступных для панели инструментов.
ms.assetid: 9040ab84-a5f3-4e4b-bc90-590b2ceeaa5a
keywords:
- элементы управления Windows сообщений TB_ADDBITMAP
topic_type:
- apiref
api_name:
- TB_ADDBITMAP
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 61b024c224ab305c4a13942c62a2de8d769d2f23b82d21ef295e024bae82f563
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119919234"
---
# <a name="tb_addbitmap-message"></a>\_Сообщение АДДБИТМАП ТБ

Добавляет одно или несколько изображений в список изображений кнопок, доступных для панели инструментов.

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Число изображений кнопок в точечном рисунке. Если аргумент *lParam* задает системный точечный рисунок, этот параметр игнорируется.

</dd> <dt>

*lParam* 
</dt> <dd>

Указатель на структуру [**тбаддбитмап**](/windows/win32/api/commctrl/ns-commctrl-tbaddbitmap) , которая содержит идентификатор ресурса точечного рисунка и маркер для экземпляра модуля с исполняемым файлом, содержащим ресурс точечного рисунка.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает индекс первого нового изображения, если выполнено успешно, или значение-1 в противном случае.

## <a name="remarks"></a>Remarks

Если панель инструментов была создана с помощью функции [**CreateWindowEx**](/windows/desktop/api/winuser/nf-winuser-createwindowexa) , перед отправкой **\_ аддбитмап ТБ** необходимо отправить на панель инструментов сообщение [**\_ буттонструктсизе**](tb-buttonstructsize.md) ТБ.

## <a name="examples"></a>Примеры

В следующем примере создается точечный рисунок из ресурса (IDB \_ BITMAP1), который сопоставляет цвет фона (черный в данном случае) с цветом лицевой кнопки системы и добавляет его на панель инструментов.


```C++
DWORD backgroundColor = GetSysColor(COLOR_BTNFACE);
COLORMAP colorMap;
colorMap.from = RGB(0, 0, 0);
colorMap.to = backgroundColor;
HBITMAP hbm = CreateMappedBitmap(g_hInst, IDB_BITMAP1, 0, &colorMap, 1);
TBADDBITMAP tb;
tb.hInst = NULL;
tb.nID = (UINT_PTR)hbm;

// hWndToolbar is the window handle of the toolbar.
// Do not forget to send TB_BUTTONSTRUCTSIZE if the toolbar was 
// created by using CreateWindowEx.
int index = SendMessage (hWndToolbar, TB_ADDBITMAP, 0, (LPARAM)&tb);
```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

