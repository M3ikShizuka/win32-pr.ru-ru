---
title: Метод Player. Лаунчурл
description: Метод Лаунчурл отправляет URL-адрес браузеру пользователя по умолчанию для подготовки к просмотру. | Метод Player. Лаунчурл
ms.assetid: 2b445e59-f884-4519-9acb-f349319429d2
keywords:
- проигрыватель Windows Media метода лаунчурл
- метод лаунчурл проигрыватель Windows Media, класс Player
- класс Player проигрыватель Windows Media, метод лаунчурл
topic_type:
- apiref
api_name:
- Player.launchURL
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 3c496e8f40f4d7c8a21e718b820e438d3ce32ad1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127172747"
---
# <a name="playerlaunchurl-method"></a>Метод Player. Лаунчурл

Метод **лаунчурл** отправляет URL-адрес браузеру пользователя по умолчанию для подготовки к просмотру.

## <a name="syntax"></a>Синтаксис


```JScript
Player.launchURL(
  URL
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*URL-адрес* \[ окне\]
</dt> <dd>

**Строковое** значение, представляющее URL-адрес для запуска.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Remarks

Этот метод открывает только веб-страницы с использованием протоколов HTTP или HTTPS.

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="examples"></a>Примеры

В следующем примере создается элемент кнопки HTML, который при нажатии отображает веб-сайт Майкрософт в новом окне браузера. Был создан элемент **Player** с идентификатором "Player".


```JScript
<INPUT  TYPE = "BUTTON"  ID = "GOTOMS"  VALUE = "Microsoft.com"  onClick = "

    /* Open the Microsoft website. */
    Player.launchURL('https://www.microsoft.com');
">

```



## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Объект Player**](player-object.md)
</dt> </dl>

 

 





