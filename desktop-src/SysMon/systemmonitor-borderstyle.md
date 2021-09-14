---
title: Системмонитор. BorderStyle, свойство
description: Возвращает или задает стиль границы элемента управления.
ms.assetid: 9151a3f6-71fb-43ea-b7f6-cc35048145cb
keywords:
- Свойство BorderStyle Сисмон
- Свойство BorderStyle Сисмон, класс Системмонитор
- Класс Системмонитор Сисмон, свойство BorderStyle
topic_type:
- apiref
api_name:
- SystemMonitor.BorderStyle
api_location:
- Sysmon.ocx
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e5dd0cec7e4d0d6d3223da4486d4569f8bc611e6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056789"
---
# <a name="systemmonitorborderstyle-property"></a>Системмонитор. BorderStyle, свойство

Возвращает или задает стиль границы элемента управления.

Это свойство доступно только для чтения.

## <a name="syntax"></a>Синтаксис


```VB
Property BorderStyle As Long
```



## <a name="property-value"></a>Значение свойства

Стиль границы элемента управления.

Для этого свойства можно задать одно из следующих значений.



| Значение                                                                                                                                                                                                                                                                                                                                                                                                   | Значение                                          |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|
| <span id="System.Windows.Forms.FormBorderStyle.VbBSNone"></span><span id="system.windows.forms.formborderstyle.vbbsnone"></span><span id="SYSTEM.WINDOWS.FORMS.FORMBORDERSTYLE.VBBSNONE"></span><dl> <dt>**Система. Windows. Forms. FormBorderStyle. Вббсноне**</dt> <dt>0</dt> </dl>                     | Нет границы. Это значение по умолчанию.<br/> |
| <span id="System.Windows.Forms.FormBorderStyle.VbFixedSingle"></span><span id="system.windows.forms.formborderstyle.vbfixedsingle"></span><span id="SYSTEM.WINDOWS.FORMS.FORMBORDERSTYLE.VBFIXEDSINGLE"></span><dl> <dt>**Система. Windows. Forms. FormBorderStyle. Вбфикседсингле**</dt> <dt>1</dt> </dl> | Фиксированная одинарная граница.<br/>                 |



 

## <a name="exceptions"></a>Исключения



| Тип исключения               | Условие                                |
|------------------------------|------------------------------------------|
| **System.ArgumentException** | Указан недопустимый стиль границы. |



 

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                            |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                  |
| DLL<br/>                      | <dl> <dt>Сисмон. ocx</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**системмонитор**](systemmonitor.md)
</dt> </dl>

 

 





