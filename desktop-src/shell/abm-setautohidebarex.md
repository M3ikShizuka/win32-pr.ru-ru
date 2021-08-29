---
description: Регистрирует или отменяет регистрацию панель приложенийа автоскрытия для заданной границы экрана. Это сообщение расширяет АБМ \_ сетаутохидебар, позволяя указать определенный монитор, который будет использоваться в ситуациях с несколькими мониторами.
title: Сообщение ABM_SETAUTOHIDEBAREX (Шеллапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.assetid: C437727C-3FF6-4598-9D81-A39FCC2EF1C4
api_name:
- ABM_SETAUTOHIDEBAREX
api_type:
- HeaderDef
api_location:
- Shellapi.h
topic_type:
- APIRef
- kbSyntax
ms.openlocfilehash: d98bbfe9566aa5edeccb7d340de28b1fa4b249d26b8ad740a718ddc5e6bc6a68
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119884824"
---
# <a name="abm_setautohidebarex-message"></a>\_Сообщение АБМ сетаутохидебарекс

Регистрирует или отменяет регистрацию панель приложенийа автоскрытия для заданной границы экрана. Это сообщение расширяет [**АБМ \_ сетаутохидебар**](abm-setautohidebar.md) , позволяя указать определенный монитор, который будет использоваться в ситуациях с несколькими мониторами.


```C++
fSuccess = (BOOL) SHAppBarMessage(ABM_SETAUTOHIDEBAR, pabd); 
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*пабд* 
</dt> <dd>

Указатель на структуру [**аппбардата**](/windows/desktop/api/Shellapi/ns-shellapi-appbardata) . Установите для члена **lParam** значение **true** , чтобы зарегистрировать панель приложений, или **false** , чтобы отменить регистрацию. При отправке этого сообщения необходимо указать члены **кбсизе**, **HWND**, **уедже**, **RC** и **lParam** . все остальные элементы игнорируются.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает **true** при успешном выполнении, или **false** , если возникла ошибка или если панель приложений автоматически был зарегистрирован для данного объекта на данном мониторе.

## <a name="remarks"></a>Remarks

Система допускает только одно автоматическое скрытие панель приложений для каждого края каждого монитора. Монитор определяется членом **RC** , а ребро определяется членом **уедже** структуры [**аппбардата**](/windows/desktop/api/Shellapi/ns-shellapi-appbardata) .

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Шеллапи. h</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**АБМ \_ жетаутохидебар**](abm-getautohidebar.md)
</dt> <dt>

[**АБМ \_ жетаутохидебарекс**](abm-getautohidebarex.md)
</dt> <dt>

[**АБМ \_ сетаутохидебар**](abm-setautohidebar.md)
</dt> </dl>

 

 




