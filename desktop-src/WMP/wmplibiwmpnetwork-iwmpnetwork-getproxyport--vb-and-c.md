---
title: Ивмпнетворк Жетпроксипорт, метод
description: Метод Жетпроксипорт Возвращает используемый порт прокси-сервера.
ms.assetid: fc94f3a9-458d-410c-98e9-a34be6e08c52
keywords:
- проигрыватель Windows Media метода жетпроксипорт
- проигрыватель Windows Media метода жетпроксипорт, интерфейс ивмпнетворк
- проигрыватель Windows Media интерфейса ивмпнетворк, метод жетпроксипорт
topic_type:
- apiref
api_name:
- IWMPNetwork.getProxyPort
api_location:
- Interop.WMPLib.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 46fb388c2740e709e75579c01d216af677a826c1
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127264704"
---
# <a name="iwmpnetworkgetproxyport-method"></a>Метод Ивмпнетворк:: Жетпроксипорт

Метод **жетпроксипорт** Возвращает используемый порт прокси-сервера.

## <a name="syntax"></a>Синтаксис


```CSharp
public System.Int32 getProxyPort(
  System.String bstrProtocol
);
```


```VB

Public Function getProxyPort( _
  ByVal bstrProtocol As System.String _
) As System.Int32
Implements IWMPNetwork.getProxyPort
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*бстрпротокол* \[ окне\]
</dt> <dd>

**Строка System. String** , которая является именем протокола. Список поддерживаемых протоколов см. в разделе [Поддерживаемые протоколы и типы файлов](supported-protocols-and-file-types.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Объект **System. Int32** , который является используемым портом прокси-сервера. Значение имеет смысл только в том случае, если **ивмпнетворк. жетпроксисеттингс** возвращает значение 2 (использовать параметры вручную).

## <a name="remarks"></a>Комментарии

Этот метод завершается ошибкой, если вызывающее приложение не выполняется на локальном компьютере или в интрасети.

## <a name="examples"></a>Примеры

в следующем примере кода используется **жетпроксипорт** для вывода текущих номеров портов прокси-сервера проигрыватель Windows Media для протоколов MMS и HTTP. Объект **аксвмплиб. аксвиндовсмедиаплайер** представлен переменной с именем Player.


```CSharp
// Variables to hold the results of calls to getProxyPort. 
int proxyPortHTTP = 0;
int proxyPortMMS = 0;

// Test whether the HTTP proxy settings are manual.
if (player.network.getProxySettings("HTTP") == 2)
{
    proxyPortHTTP = player.network.getProxyPort("HTTP");
}

// Test whether the MMS proxy settings are manual.
if (player.network.getProxySettings("MMS") == 2)
{
    proxyPortMMS = player.network.getProxyPort("MMS");
}

// Store the proxy port numbers in a string array and display them using a multi-line
// text box. Unavailable proxy port numbers will display as "undefined".
proxyPorts[0] = ("The current HTTP proxy port is: " + proxyPortHTTP.ToString());
proxyPorts[1] = ("The current MMS proxy port is: " + proxyPortMMS.ToString());
proxyPortText.Lines = proxyPorts;
```


```VB

' Variables to hold the results of calls to getProxyPort. 
Dim proxyPortHTTP As Integer = 0
Dim proxyPortMMS As Integer = 0

&#39; Test whether the HTTP proxy settings are manual.
If (player.network.getProxySettings(&quot;HTTP&quot;) = 2) Then

    proxyPortHTTP = player.network.getProxyPort(&quot;HTTP&quot;)

End If

&#39; Test whether the MMS proxy settings are manual.
If (player.network.getProxySettings(&quot;MMS&quot;) = 2) Then

    proxyPortMMS = player.network.getProxyPort(&quot;MMS&quot;)

End If

&#39; Store the proxy port numbers in a string array and display them using a multi-line
&#39; text box. Unavailable proxy port numbers will display as &quot;undefined&quot;.
proxyPorts(0) = (&quot;The current HTTP proxy port is: &quot; + proxyPortHTTP.ToString())
proxyPorts(1) = (&quot;The current MMS proxy port is: &quot; + proxyPortMMS.ToString())
proxyPortText.Lines = proxyPorts
```





## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------|------------------------------------------------------------------------------------------------------------------------|
| Версия<br/>   | проигрыватель Windows Media 9 Series или более поздней версии<br/>                                                                      |
| Пространство имен<br/> | **вмплиб**<br/>                                                                                                  |
| Сборка<br/>  | <dl> <dt>Interop.WMPLib.dll (Interop.WMPLib.dll.dll)</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Ивмпнетворк (VB и C#)**](iwmpnetwork--vb-and-c.md)
</dt> <dt>

[**Ивмпнетворк. Жетпроксисеттингс (VB и C#)**](wmplibiwmpnetwork-iwmpnetwork-getproxysettings--vb-and-c.md)
</dt> <dt>

[**Ивмпнетворк. Сетпроксипорт (VB и C#)**](wmplibiwmpnetwork-iwmpnetwork-setproxyport--vb-and-c.md)
</dt> </dl>

 

 





