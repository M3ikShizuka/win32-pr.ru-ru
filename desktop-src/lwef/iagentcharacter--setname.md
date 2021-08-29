---
title: Иажентчарактер SetName
description: Иажентчарактер SetName
ms.assetid: 4944f910-60e9-446b-82e9-2794f445789a
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d46a2210b14519a0595f37786725559d363cddaceb62ae93b80a52deb839e0b6
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119725294"
---
# <a name="iagentcharactersetname"></a>Иажентчарактер:: SetName

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT SetName(
   BSTR bszName   // character name
);
```

Задает имя символа.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="bszName"></span><span id="bszname"></span><span id="BSZNAME"></span>*бсзнаме*
</dt> <dd>

Значение типа BSTR, задающее имя символа. Имя символа по умолчанию определяется при компиляции с помощью редактора символов Microsoft Agent. Его можно изменить с помощью **иажентчарактер:: SetName**; Однако это изменяет имя символа для всех текущих клиентов символа. Это свойство не является постоянным (хранится без возможности восстановления). Имя символа возвращается к имени по умолчанию при первой загрузке символа клиентом.

Имя символа может также зависеть от идентификатора языка. Символы могут быть скомпилированы с разными именами для разных языков.

Сервер использует параметр имени символа в частях интерфейса Microsoft Agent, например, заголовок окна «Voice Commands», если символ является входным и находится во всплывающем меню Microsoft Agent панели задач.

</dd> </dl>

## <a name="see-also"></a>См. также:

[**Иажентчарактер:: Name**](iagentcharacter--getname.md)


 

 




