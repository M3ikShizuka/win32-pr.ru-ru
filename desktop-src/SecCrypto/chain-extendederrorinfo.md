---
description: Возвращает строку, содержащую дополнительные сведения об ошибке индексированной записи.
ms.assetid: 4f0d5289-c414-4e2b-b612-be8ce1d98b12
title: 'Метод IChain2:: Екстендедерроринфо'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Chain.ExtendedErrorInfo
- IChain2.ExtendedErrorInfo
api_type:
- COM
api_location:
- Capicom.dll
ms.openlocfilehash: 460e16fd99a8599927e80c2e737ed35c5eb1e138899f83c4450ae2220d67f7fa
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119876935"
---
# <a name="ichain2extendederrorinfo-method"></a>Метод IChain2:: Екстендедерроринфо

\[CAPICOM — это 32-разрядный компонент, доступный для использования в следующих операционных системах: Windows Server 2008, Windows Vista и Windows XP. Вместо этого используйте [**класс X509Chain**](/dotnet/api/system.security.cryptography.x509certificates.x509chain?view=netcore-3.1) в пространстве имен [**System. Security. Cryptography. X509Certificates**](/dotnet/api/system.security.cryptography.x509certificates.publickey.-ctor?view=netcore-3.1) .\]

Метод **екстендедерроринфо** возвращает строку, которая содержит дополнительные сведения об ошибке индексированной записи.

Этот метод появился в CAPICOM 2,0.

## <a name="syntax"></a>Синтаксис


```VB
Chain.ExtendedErrorInfo( _
  [ ByVal Index ] _
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Индекс* \[ в необязательное\]
</dt> <dd>

Значение **типа Long** , представляющее индекс записи. Значение по умолчанию — 1, возвращающее сведения об ошибке для конечного сертификата в цепочке. **Certificates. Count** возвращает сведения о корневом сертификате цепочки. 0 возвращает расширенные сведения об ошибке для всей цепочки.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Строка, содержащая расширенные сведения об ошибке.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|----------------------------------|----------------------------------------------------------------------------------------|
| Окончание поддержки клиента<br/> | Windows Vista<br/>                                                               |
| Поддержка конца сервера<br/> | Windows Server 2008<br/>                                                         |
| Распространяемые компоненты<br/>       | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Цепочк**](chain.md)
</dt> </dl>

 

 
