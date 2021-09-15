---
description: Структура, описывающая одно значение цвета.
ms.assetid: 710f3ef1-bbc3-416d-9faf-aa4a716007c2
title: XPS_COLOR (Кспсобжектмодел. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 34c148c2a5452154bfe33b0c74d695fe78f0cdad
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127570527"
---
# <a name="xps_color"></a>\_Цвет XPS

Структура, описывающая одно значение цвета.

``` syntax
typedef union switch (XPS_COLOR_TYPE colorType) value
{
    case XPS_COLOR_TYPE_SRGB:
        struct {
            byte alpha, red, green, blue;
        } sRGB;
    case XPS_COLOR_TYPE_SCRGB:
        struct {
            FLOAT alpha, red, green, blue;
        } scRGB;
    case XPS_COLOR_TYPE_CONTEXT:
        struct {
            byte channelCount;
            FLOAT channels[9];
        } context;
} XPS_COLOR;
```

## <a name="remarks"></a>Remarks

Формат структуры зависит от значения *колортипе*.

<dl>

[**\_Тип цвета \_ XPS \_ sRGB**](/previous-versions/windows/desktop/dd372944(v=vs.85))  
[**\_Тип цвета \_ XPS \_ SCRGB**](/previous-versions/windows/desktop/dd372943(v=vs.85))  
[**\_ \_ контекст типа цвета \_ XPS**](/windows/win32/api/xpsobjectmodel/ns-xpsobjectmodel-xps_color)  
</dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 7, Windows Vista с пакетом обновления 2 (SP2) и обновлением платформы для приложений для \[ классических приложений Windows Vista \|\]<br/>                          |
| Минимальная версия сервера<br/> | Windows сервер 2008 R2, Windows Server 2008 с пакетом обновления 2 (SP2) и обновлением платформы для Windows Server 2008 приложения \[ UWP для классических приложений \|\]<br/> |
| Заголовок<br/>                   | <dl> <dt>Кспсобжектмодел. h</dt> </dl>                                              |
| IDL<br/>                      | <dl> <dt>Кспсобжектмодел. idl</dt> </dl>                                            |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[XPS](https://www.ecma-international.org/activities/XML%20Paper%20Specification/XPS%20Standard%20WD%201.6.pdf)
</dt> </dl>

 

