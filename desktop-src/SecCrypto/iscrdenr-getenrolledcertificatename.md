---
description: 'Возвращает имя сертификата, полученное в результате предыдущего успешного вызова Искрденр:: RECALL.'
ms.assetid: e33b217a-b717-49bd-b0f3-3ba9229a0696
title: 'Метод Искрденр:: Жетенролледцертификатенаме'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ISCrdEnr.getEnrolledCertificateName
- SCrdEnr.getEnrolledCertificateName
api_type:
- COM
api_location:
- Scrdenrl.dll
ms.openlocfilehash: e3c9640e7719d2b5ac0e576384246cda5e1b2bfe
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127347919"
---
# <a name="iscrdenrgetenrolledcertificatename-method"></a>Метод Искрденр:: Жетенролледцертификатенаме

Метод **жетенролледцертификатенаме** извлекает имя сертификата, полученного при предыдущем успешном вызове [**искрденр::**](/previous-versions/windows/desktop/legacy/aa386564(v=vs.85))Recall.

Этот метод также можно использовать для вывода сертификата в диалоговом окне. Этот метод вызывает функцию [*CryptoAPI*](../secgloss/c-gly.md) [**цертжетнаместринг**](/windows/desktop/api/Wincrypt/nf-wincrypt-certgetnamestringa).

## <a name="syntax"></a>Синтаксис


```C++
HRESULT getEnrolledCertificateName(
  [in]  DWORD     dwFlags,
  [out] BSTR *pBstrCertName
);
```


```VB

SCrdEnr.getEnrolledCertificateName( _
  ByVal dwFlags, _
  ByRef pBstrCertName _
)
```





## <a name="parameters"></a>Параметры

<dl> <dt>

*dwFlags* \[ окне\]
</dt> <dd>

Значение, определяющее, отображается ли сертификат в диалоговом окне. Если это значение равно бросить \_ Регистрация \_ не \_ отображает \_ сертификат (определенный как 0x01), зарегистрированный сертификат не отображается; любые другие значения приводят к отображению зарегистрированного сертификата в диалоговом окне **сертификат** .

</dd> <dt>

*пбстрцертнаме* \[ заполняет\]
</dt> <dd>

Указатель на строку, которая возвращает полученное имя сертификата.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

### <a name="c"></a>C++

Если метод завершается успешно, метод возвращает значение S \_ ОК.

Если метод завершается с ошибкой, возвращается значение **HRESULT** , указывающее на ошибку. Список распространенных кодов ошибок см. в разделе [Общие значения HRESULT](common-hresult-values.md).

### <a name="vb"></a>VB

Строка, представляющая полученное имя сертификата.

## <a name="remarks"></a>Remarks

Так как этот метод работает с существующим сертификатом, необходимо успешно вызвать [**искрденр::**](/previous-versions/windows/desktop/legacy/aa386564(v=vs.85)) Call, прежде чем можно будет вызвать **жетенролледцертификатенаме**.

Метод **жетенролледцертификатенаме** вызывает функцию [**цертжетнаместринг**](/windows/desktop/api/Wincrypt/nf-wincrypt-certgetnamestringa) для получения имени сертификата в соответствии с последовательностью, описанной для \_ \_ \_ значения простого отображаемого типа сертификата для \_ параметра **цертжетнаместринг** *двтипе* .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                               |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| DLL<br/>                      | <dl> <dt>Scrdenrl.dll</dt> </dl> |
| IID<br/>                      | IID \_ искрденр определен как 753988a1-1357-436d-9cf5-f089bdd67d64<br/>             |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**искрденр**](iscrdenr.md)
</dt> <dt>

[**Искрденр:: регистрация**](/previous-versions/windows/desktop/legacy/aa386564(v=vs.85))
</dt> </dl>

 

 
