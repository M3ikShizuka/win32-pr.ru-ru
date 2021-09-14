---
description: Метод Двдадм. Жетпаренталлевел получает родительский уровень, который был сохранен в реестре в последний раз.
ms.assetid: 2aadcf41-2c65-4f3a-8ce8-0fc9aa580ad9
title: Метод Жетпаренталлевел
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: fdfa2c2193a9d02249076b2be2225fc50cd1edd5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127053366"
---
# <a name="getparentallevel-method"></a>Метод Жетпаренталлевел

> [!Note]  
> этот компонент доступен для использования в операционных системах Microsoft Windows 2000, Windows XP и Windows Server 2003. В последующих версиях он может быть изменен или недоступен.

 

`DVDAdm.GetParentalLevel`Метод получает родительский уровень, который был сохранен в реестре последним.

``` syntax
[ iParentalLevel = ] DVD.DVDAdm.GetParentalLevel()
```

## <a name="return-value"></a>Возвращаемое значение

Возвращает целое число от 1 до 8, указывающее на родительский уровень по умолчанию.

## <a name="remarks"></a>Комментарии

Родительский уровень, получаемый этим методом, не обязательно является тем же уровнем, который в настоящее время хранится в элементе управления Мсвебдвд; чтобы получить уровень, хранящийся в данный момент в элементе управления, вызовите метод [**жетплайерпаренталлевел**](getplayerparentallevel-method.md) . Значение-1 указывает на то, что функция родительского управления отключена.

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Объект Мсдвдадм](msdvdadm-object.md)
</dt> </dl>

 

 



