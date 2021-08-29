---
description: Связывает реализацию Итрансактионпрокси с текущим контекстом.
ms.assetid: 64009632-b536-41fb-95ac-b23e2cbf18da
title: 'Метод Иконтексттрансактионинфо:: Регистертрансактионпрокси'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IContextTransactionInfo.RegisterTransactionProxy
api_type:
- COM
api_location: ''
ms.openlocfilehash: 7bdae305fc7dc7ec15c2d140064d7479e4454d1bdb04562f5dd4201a92072425
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119954024"
---
# <a name="icontexttransactioninforegistertransactionproxy-method"></a>Метод Иконтексттрансактионинфо:: Регистертрансактионпрокси

Связывает реализацию [**итрансактионпрокси**](/windows/desktop/api/ComSvcs/nn-comsvcs-itransactionproxy) с текущим контекстом.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT RegisterTransactionProxy(
  [in]  ITransactionProxy *pProxy,
  [out] GUID              *pGuid
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппрокси* \[ окне\]
</dt> <dd>

Реализация [**итрансактионпрокси**](/windows/desktop/api/ComSvcs/nn-comsvcs-itransactionproxy) , связываемая с текущим контекстом.

</dd> <dt>

*пгуид* \[ заполняет\]
</dt> <dd>

Идентификатор GUID, определяющий прокси транзакции. COM+ использует этот идентификатор GUID при вызове [**итрансактионпрокси:: Commit**](/windows/desktop/api/ComSvcs/nf-comsvcs-itransactionproxy-commit) на прокси транзакции.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод может возвращать стандартные возвращаемые значения E \_ INVALIDARG, e \_ OUTOFMEMORY и e с \_ непредвиденными значениями, а также следующие значения.



| Код возврата                                                                                                     | Описание                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| <dl> <dt>**\_ОК**</dt> </dl>                            | Метод завершился успешно.<br/>                                                                           |
| <dl> <dt>**КОНТЕКСТ \_ E \_ алреадинтрансактион**</dt> </dl> | У текущего контекста уже есть связанная реализация [**итрансактионпрокси**](/windows/desktop/api/ComSvcs/nn-comsvcs-itransactionproxy) .<br/> |
| <dl> <dt>**E \_ нотимпл**</dt> </dl>                       | В текущем контексте размещается транзакция "присвоить собственную транзакцию" (BYOT) или некорневая транзакция.<br/>    |



 

## <a name="remarks"></a>Remarks

Метод **регистертрансактионпрокси** может быть вызван только в том случае, если текущий контекст является корневым контекстом транзакции. Он не может быть вызван, если в контексте размещается транзакция BYOT или некорневая транзакция.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP с пакетом обновления 2 (SP2) \[ только классические приложения\]<br/>          |
| Минимальная версия сервера<br/> | Windows Только для настольных приложений сервера 2003 с пакетом обновления 1 \[\]<br/> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**иконтексттрансактионинфо**](icontexttransactioninfo.md)
</dt> </dl>

 

 




