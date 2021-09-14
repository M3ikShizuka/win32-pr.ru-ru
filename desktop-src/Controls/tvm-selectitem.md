---
title: Сообщение TVM_SELECTITEM (Коммктрл. h)
description: Выбирает указанный элемент представления дерева, прокручивает элемент в представлении или перерисовывает элемент в стиле, который используется для указания цели операции перетаскивания.
ms.assetid: 8b943958-7b93-4e54-99de-200121cf0752
keywords:
- элементы управления Windows сообщений TVM_SELECTITEM
topic_type:
- apiref
api_name:
- TVM_SELECTITEM
api_location:
- Commctrl.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 0ec7201358669fa49e6396508d371ca5e95d6fa1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127165672"
---
# <a name="tvm_selectitem-message"></a>\_Сообщение TVM селектитем

Выбирает указанный элемент представления дерева, прокручивает элемент в представлении или перерисовывает элемент в стиле, который используется для указания цели операции перетаскивания. Это сообщение можно отправить явным образом или с помощью макроса [**\_ SELECT TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_select), [**TreeView \_ селектитем**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_selectitem)или [**TreeView \_ селектдроптаржет**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_selectdroptarget) .

## <a name="parameters"></a>Параметры

<dl> <dt>

*wParam* 
</dt> <dd>

Флаг действия. Этот параметр может принимать одно из следующих значений:




| Значение | Значение | 
|-------|---------|
| <span id="TVGN_CARET"></span><span id="tvgn_caret"></span><dl><dt><strong>TVGN_CARET</strong></dt></dl> | Задает выборку для указанного элемента. Родительское окно элемента управления представлением дерева получает <a href="tvn-selchanging.md">TVN_SELCHANGING</a> и <a href="tvn-selchanged.md">TVN_SELCHANGED</a> коды уведомления. <br /> | 
| <span id="TVGN_DROPHILITE"></span><span id="tvgn_drophilite"></span><dl><dt><strong>TVGN_DROPHILITE</strong></dt></dl> | Перерисовывает указанный элемент в стиле, который используется для указания цели операции перетаскивания.<br /> | 
| <span id="TVGN_FIRSTVISIBLE"></span><span id="tvgn_firstvisible"></span><dl><dt><strong>TVGN_FIRSTVISIBLE</strong></dt></dl> | Гарантирует, что указанный элемент является видимым, и, если это возможно, отображает его в верхней части окна элемента управления. Элементы управления "дерево-представление" отображают столько элементов, сколько будет помещаться в окне. Если указанный элемент находится ближе к нижней части иерархии элементов управления, он может не стать первым видимым элементом в зависимости от того, сколько элементов умещается в окне.<br /> | 
| <span id="TVSI_NOSINGLEEXPAND"></span><span id="tvsi_nosingleexpand"></span><dl><dt><strong>TVSI_NOSINGLEEXPAND</strong></dt></dl> | Если выбран один элемент, гарантирует, что TreeView не расширяет его дочерние элементы. Это допустимо, только если используется с флагом TVGN_CARET. <br /><blockquote>[!Note]<br />Чтобы использовать этот флаг, необходимо указать манифест, задающий Comclt32.dll версии 6,0. Дополнительные сведения о манифестах см. в разделе <a href="cookbook-overview.md">Включение визуальных стилей</a>.</blockquote><br /> | 




 

</dd> <dt>

*lParam* 
</dt> <dd>

Обработчик элемента. Если параметр *lParam* имеет **значение NULL**, элементу управления задается значение, не имеющее выбранного элемента.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **значение true** , если успешно, или **false** в противном случае.

## <a name="remarks"></a>Remarks

Если указанный элемент является дочерним по отношению к свернутому родительскому элементу, то родительский список дочерних элементов разворачивается для отображения указанного элемента. В этом случае родительское окно элемента управления получает коды уведомлений [ТВН \_ Итемекспандинг](tvn-itemexpanding.md) и [ТВН \_ итемекспандед](tvn-itemexpanded.md) .

Использование макроса [**\_ Селектитем в TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_selectitem) эквивалентно отправке **сообщения \_ Селектитем TVM** с параметром *wParam* , равным \_ значению курсора твгн. Использование макроса [**\_ Селектдроптаржет в TreeView**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_selectdroptarget) эквивалентно отправке сообщения **TVM \_ селектитем** с параметром *wParam* , равным \_ значению твгн дрофилите. Использование [**TreeView \_ селектсетфирствисибле**](/windows/desktop/api/Commctrl/nf-commctrl-treeview_selectsetfirstvisible) эквивалентно отправке сообщения **TVM \_ селектитем** с параметром *wParam* , установленным в \_ значение твгн фирствисибле.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                        |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                  |
| Заголовок<br/>                   | <dl> <dt>Коммктрл. h</dt> </dl> |



 

 





