---
title: Тело интерфейса IDL
description: Текст интерфейса IDL содержит типы данных, используемые в удаленных вызовах процедур, и прототипы функций для удаленных процедур.
ms.assetid: b07524a7-b27e-4ea2-ae34-068c07d9a444
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2a25f1e74a1c0e33d0f3bde1318a36e8825fc350c445ee079ad534b67af51c03
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120017064"
---
# <a name="the-idl-interface-body"></a>Тело интерфейса IDL

Текст интерфейса IDL содержит типы данных, используемые в удаленных вызовах процедур, и прототипы функций для удаленных процедур. Тело интерфейса может также содержать импорты, прагмы, объявления констант и объявления типов. В режиме расширений Microsoft компилятор MIDL также допускает неявные объявления в форме определений переменных.

В следующем примере показан IDL-файл, содержащий определение интерфейса. Текст определения интерфейса, который находится между фигурными скобками, содержит определение константы (**буфсизе**), тип (**\_ \_ тип обработчика пконтекст**) и некоторые удаленные процедуры (**ремотеопен**, **ремотереад**, **ремотеклосе** и **Shutdown**).

``` syntax
[ 
  uuid (ba209999-0c6c-11d2-97cf-00c04f8eea45), 
  version(1.0), 
  pointer_default(unique) 
] 
interface cxhndl 
{ 
 
  const short BUFSIZE = 1024;  
 
  typedef [context_handle] void *PCONTEXT_HANDLE_TYPE; 
 
  short RemoteOpen( 
      [out] PCONTEXT_HANDLE_TYPE *pphContext, 
      [in, string] unsigned char *pszFile 
  ); 
 
   short RemoteRead( 
      [in]  PCONTEXT_HANDLE_TYPE phContext, 
      [out] unsigned char achBuf[BUFSIZE], 
      [out] short *pcbBuf 
  ); 
 
  short RemoteClose( [in, out] PCONTEXT_HANDLE_TYPE *pphContext ); 
 
  void Shutdown(void); 
 
}
```

Дополнительные сведения см. в [справочнике по языку MIDL](/windows/desktop/Midl/midl-language-reference).

 

 