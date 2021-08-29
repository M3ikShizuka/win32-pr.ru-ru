---
description: Интерфейс Иенумпсторетипес — предоставляет стандартные методы перечисления COM для интерфейса Ипсторе.
ms.assetid: a90bc5cf-ca42-4007-a57b-be9c59d9552a
title: Интерфейс Иенумпсторетипес (PStore. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IEnumPStoreTypes
api_type:
- COM
api_location:
- Pstorec.dll
ms.openlocfilehash: 668ed2b7177344004cb4b872ff47a5924fdcc1778cfbfbb3c6d3d447b624546c
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "118955963"
---
# <a name="ienumpstoretypes-interface"></a>Интерфейс Иенумпсторетипес

\[защищенные служба хранилища (Pstore) доступны для использования в Windows Server 2003 и Windows XP. она доступна только для операций чтения в Windows Server 2008 и Windows Vista, но может быть недоступна в последующих версиях. PStore использует старую реализацию защиты данных. Разработчикам настоятельно рекомендуется использовать преимущества более надежной защиты данных, предоставляемые функциями [**CryptProtectData**](/windows/win32/api/dpapi/nf-dpapi-cryptprotectdata) и [**CryptUnprotectData**](/windows/win32/api/dpapi/nf-dpapi-cryptunprotectdata) .\]

Предоставляет стандартные методы перечисления COM для интерфейса [**ипсторе**](ipstore.md) .

## <a name="members"></a>Элементы

Интерфейс **иенумпсторетипес** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **Иенумпсторетипес** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **иенумпсторетипес** содержит следующие методы.



| Метод                                  | Описание                                                                                        |
|:----------------------------------------|:---------------------------------------------------------------------------------------------------|
| [**Клонировать**](ienumpstoretypes-clone.md) | Создает другой перечислитель с тем же состоянием перечисления, что и текущий.<br/> |
| [**Далее**](ienumpstoretypes-next.md)   | Возвращает следующий указанный тип поставщика в последовательности перечисления.<br/>                      |
| [**Перезапуск**](ienumpstoretypes-reset.md) | Выполняет сброс до начала последовательности перечисления.<br/>                                    |
| [**Сразу**](ienumpstoretypes-skip.md)   | Пропускает указанный тип поставщика в последовательности перечисления.<br/>                          |



 

## <a name="remarks"></a>Remarks

Объект перечислителя должен быть освобожден, если он больше не используется.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------|----------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>PStore. h</dt> </dl>    |
| DLL<br/>    | <dl> <dt>Pstorec.dll</dt> </dl> |



 

 
