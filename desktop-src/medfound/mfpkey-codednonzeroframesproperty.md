---
description: Указывает количество видеокадров, закодированных кодеком, который фактически содержит данные.
ms.assetid: f96fd0b2-8c81-4318-b44c-4b794b3945a3
title: Свойство MFPKEY_CODEDNONZEROFRAMES (Вмкодекдсп. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: e1263a15d9ddd678360bf57f5f704143d580d6b17ab63af0777c20d9b09204cd
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119954684"
---
# <a name="mfpkey_codednonzeroframes-property"></a>МФПКЭЙ \_ кодеднонзерофрамес, свойство

Указывает количество видеокадров, закодированных кодеком, который фактически содержит данные.

## <a name="constant-for-ipropertybag"></a>Константа для Ипропертибаг

Доступно только с помощью [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore).

## <a name="data-type"></a>Тип данных

VT \_ I4

## <a name="remarks"></a>Remarks

Это значение равно [мфпкэй \_ тоталфрамес](mfpkey-totalframesproperty.md) минус все кадры, которые были удалены из-за ограничений битовой частоты, за вычетом кадров нулевых байтов. Это значение можно получить после завершения передачи образцов. Для повторяющихся кадров можно создавать кадры нулевого байта.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                             |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                    |
| Заголовок<br/>                   | <dl> <dt>Вмкодекдсп. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Свойства Media Foundation](media-foundation-properties.md)
</dt> </dl>

 

 
