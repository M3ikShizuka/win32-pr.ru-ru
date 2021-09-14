---
title: атрибут ncacn_nb_ipx
description: '\_ \_ Ключевое слово нкакн NetBIOS IPX определяет NetBIOS через IPX в качестве семейства протоколов для конечной точки. Это семейство протоколов устарело и не должно использоваться в новых приложениях.'
ms.assetid: 641471d4-eba4-4d4a-a3fe-1e40b3751e38
keywords:
- ncacn_nb_ipx атрибута MIDL
topic_type:
- apiref
api_name:
- ncacn_nb_ipx
api_type:
- NA
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 156b5c460c4cc8638640e7eb3500ec9a7a9fa0b0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127143618"
---
# <a name="ncacn_nb_ipx-attribute"></a>\_ \_ атрибут IPX нкакн NetBIOS

Ключевое слово **нкакн \_ NetBIOS \_ IPX** определяет NetBIOS через IPX в качестве семейства протоколов для конечной точки. Это семейство протоколов устарело и не должно использоваться в новых приложениях.

``` syntax
endpoint("ncacn_nb_ipx:[port-name]")
```

## <a name="parameters"></a>Параметры

<dl> <dt>

*имя порта* 
</dt> <dd>

Задает необязательное 8-разрядное значение в диапазоне от 1 до 254. Значения меньше 0x20 зарезервированы. Если значение *имени порта* не указано, служба сопоставления конечных точек выбирает значение порта.

</dd> </dl>

## <a name="remarks"></a>Remarks

Синтаксис строки порта NetBIOS, как и все строки портов, определяется реализацией транспорта и не зависит от спецификации IDL. Компилятор MIDL выполняет ограниченную проверку синтаксиса, но не гарантирует, что указана правильная спецификация конечной точки. Некоторые классы ошибок могут выводиться во время выполнения, а не во время компиляции.

> [!Note]  
> Это семейство протоколов не поддерживается в Windows XP.

 

## <a name="examples"></a>Примеры

``` syntax
[
    uuid(12345678-4000-2006-0000-20000000001a), 
    version(1.1), 
    endpoint("ncacn_nb_ipx:[100]") 
] 
interface iface
{
    // Interface definition statements.
}
```

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**конечной**](endpoint.md)
</dt> <dt>

[Файл определения интерфейса (IDL)](interface-definition-idl-file.md)
</dt> <dt>

[**нкакн \_ IP \_ TCP**](ncacn-ip-tcp.md)
</dt> <dt>

[**нкакн \_ NetBIOS, \_ протокол TCP**](ncacn-nb-tcp.md)
</dt> <dt>

[**нкакн \_ имена \_ NetBIOS**](ncacn-nb-nb.md)
</dt> <dt>

[**нкакн \_ в \_ DSP**](ncacn-at-dsp.md)
</dt> <dt>

[**нкакн \_ SPX**](ncacn-spx.md)
</dt> <dt>

[**нкакн \_ NP**](ncacn-np.md)
</dt> <dt>

[**нкалрпк**](ncalrpc.md)
</dt> <dt>

[**нкадг \_ IP \_ UDP**](ncadg-ip-udp.md)
</dt> <dt>

[**нкадг \_ IPX**](ncadg-ipx.md)
</dt> <dt>

[**Строковая привязка**](/windows/desktop/Rpc/string-binding)
</dt> </dl>

 

 