---
title: Метод Network. Жетпроксипорт
description: Метод Жетпроксипорт извлекает используемый порт прокси-сервера.
ms.assetid: 76771750-3763-4029-b194-d8567b5f365e
keywords:
- проигрыватель Windows Media метода жетпроксипорт
- проигрыватель Windows Media метода жетпроксипорт, класс сети
- класс проигрыватель Windows Media сети, метод жетпроксипорт
topic_type:
- apiref
api_name:
- Network.getProxyPort
api_location:
- wmp.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 83937bcb5d8180085ab97bfd71a0cb1653a65e8bca8cead952e4bf24e10ee690
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119054592"
---
# <a name="networkgetproxyport-method"></a>Метод Network. Жетпроксипорт

Метод **жетпроксипорт** извлекает используемый порт прокси-сервера.

## <a name="syntax"></a>Синтаксис


```JScript
retVal = Network.getProxyPort(
  protocol
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*протокол* \[ окне\]
</dt> <dd>

**Строка** , указывающая имя протокола. Список поддерживаемых протоколов см. в разделе [Поддерживаемые протоколы и типы файлов](supported-protocols-and-file-types.md).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает **число** (**Long**), содержащее используемый порт прокси-сервера. Возвращаемое значение имеет смысл только в том случае, если **жетпроксисеттингс** возвращает значение 2 (использовать параметры вручную).

## <a name="remarks"></a>Remarks

Этот метод завершается ошибкой, если вызывающее приложение не выполняется на локальном компьютере или в интрасети.

**проигрыватель Windows Media 10 Mobile:** Этот метод не поддерживается.

## <a name="examples"></a>Примеры

в следующем примере JScript используется *сеть*. **жетпроксипорт** для вывода текущих номеров портов прокси-сервера проигрыватель Windows Media для протоколов MMS и HTTP. Объект **Player** создан с идентификатором "Player".


```JScript
// Test whether the HTTP proxy settings are manual.
if (Player.network.getProxySettings("HTTP") == 2)

   // Get the proxy port number for HTTP.
   var proxyPortHTTP = Player.network.getProxyPort("HTTP");

// Test whether the MMS proxy settings are manual.
if (Player.network.getProxySettings("MMS") == 2)

   // Get the proxy port number for MMS.
   var proxyPortMMS = Player.network.getProxyPort("MMS");

// Display the port numbers in the browser client area.
// Unavailable port numbers will display as "undefined".
document.write("The current HTTP proxy port is: " + proxyPortHTTP);
document.write("<BR>");
document.write("The current MMS proxy port is: " + proxyPortMMS);

```



## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media версии 7,0 или более поздней.<br/>                              |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Сетевой объект**](network-object.md)
</dt> <dt>

[**Network. Жетпроксисеттингс**](network-getproxysettings.md)
</dt> </dl>

 

 





