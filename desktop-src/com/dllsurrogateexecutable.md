---
title: дллсуррогатиксекутабле
description: Позволяет серверам DLL выполняться в пользовательском суррогатном процессе в сочетании со значением реестра Дллсуррогате. Если Дллсуррогатиксекутабле не указан, COM передает значение NULL в качестве значения первого параметра функции CreateProcess.
ms.assetid: faf5dde3-bd67-447b-a88c-e8660dc5228e
keywords:
- COM-значение реестра Дллсуррогатиксекутабле
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 877297673b0a518006ecf903f447984f9023da34
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127343018"
---
# <a name="dllsurrogateexecutable"></a>дллсуррогатиксекутабле

Позволяет серверам DLL выполняться в пользовательском суррогатном процессе в сочетании со значением реестра [**дллсуррогате**](dllsurrogate.md) . Если **дллсуррогатиксекутабле** не указан, com передает значение **null** в качестве значения первого параметра функции [**CreateProcess**](/windows/desktop/api/processthreadsapi/nf-processthreadsapi-createprocessa) .

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\AppID
   {AppID_GUID}
      DllSurrogateExecutable = file
```

## <a name="remarks"></a>Remarks

Это значение имеет тип **reg \_ SZ**. Он работает в сочетании со значением [**дллсуррогате**](dllsurrogate.md) , чтобы предотвратить неоднозначность при использовании функции [**CreateProcess**](/windows/desktop/api/processthreadsapi/nf-processthreadsapi-createprocessa) . **Дллсуррогате** указывает, нужно ли использовать пользовательский суррогат, и эти сведения передаются как первый параметр для **CreateProcess**. В зависимости от реализации **CreateProcess** эта информация может быть неоднозначной. Если указан параметр **дллсуррогатиксекутабле** , com передает значение в качестве первого параметра **CreateProcess**. Если **дллсуррогатиксекутабле** не указан, com передает значение **null** в качестве значения для первого параметра **CreateProcess**.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[**корегистерсуррогате**](/windows/desktop/api/combaseapi/nf-combaseapi-coregistersurrogate)
</dt> <dt>

[Суррогаты библиотеки DLL](dll-surrogates.md)
</dt> <dt>

[**дллсуррогате**](dllsurrogate.md)
</dt> <dt>

[**исуррогате**](/windows/win32/api/objidlbase/nn-objidlbase-isurrogate)
</dt> </dl>

 

 