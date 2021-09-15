---
title: Ивмперрор, метод
description: метод веб-справки открывает страницу проигрыватель Windows Media Web help для вывода дополнительных сведений о первой ошибке в очереди ошибок (нулевой индекс). | Ивмперрор, метод
ms.assetid: 30fc765a-04b2-44e5-99d8-0b4720ccbb25
keywords:
- проигрыватель Windows Media метода "справка"
- проигрыватель Windows Media метода "справка", интерфейс ивмперрор
- проигрыватель Windows Media интерфейса ивмперрор, метод webmethod
topic_type:
- apiref
api_name:
- IWMPError.webHelp
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 6c9b0cd48d45ac5e5e5d77d0150b8acdf13347e2
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127457961"
---
# <a name="iwmperrorwebhelp-method"></a>Метод Ивмперрор:: Help

метод веб- **справки** открывает страницу проигрыватель Windows Media Web help для вывода дополнительных сведений о первой ошибке в очереди ошибок (нулевой индекс).

## <a name="syntax"></a>Синтаксис


```CSharp
public void webHelp();
```


```VB

Public Sub webHelp()
Implements IWMPError.webHelp
```





## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="remarks"></a>Комментарии

страницы веб-справки всегда содержат последние и более подробные сведения об ошибках проигрыватель Windows Media. Этот метод автоматически передает другие сведения, необходимые для веб-справки, например используемую версию операционной системы.

Чтобы получить доступ к страницам веб-справки напрямую, используйте следующий код ошибки и ссылки центра поддержки:

-   [проигрыватель Windows Media Сведения о коде ошибки](https://support.microsoft.com/kb/886273)
-   [проигрыватель Windows Media Центр решений](https://support.microsoft.com/ph/7763#tab0)

## <a name="examples"></a>Примеры

в следующем примере создается кнопка, которая запускает страницу веб-справки Microsoft проигрыватель Windows Media в браузере. Объект Аксвмплиб. Аксвиндовсмедиаплайер представлен переменной с именем Player.


```CSharp
private void webHelpButton_Click(object sender, System.EventArgs e)
{
    // Launch the Microsoft Windows Media Player Web Help page in the browser.
    player.Error.webHelp();
}
```


```VB

Public Sub webHelpButton_Click(ByVal sender As Object, ByVal e As System.EventArgs) Handles webHelpButton.Click

    &#39; Launch the Microsoft Windows Media Player Web Help page in the browser.
    player.Error.webHelp()

End Sub
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмперрор (VB и C#)**](iwmperror--vb-and-c.md)
</dt> </dl>

 

 





