---
description: 'Дополнительные сведения: JET_SNT'
title: JET_SNT
TOCTitle: JET_SNT
ms:assetid: 74ac5142-8102-4dd3-8f2a-786a7a2ac78f
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269294(v=EXCHG.10)
ms:contentKeyID: 32765586
ms.date: 04/11/2016
ms.topic: reference
api_name: ''
topic_type:
- apiref
- kbArticle
api_type:
- COM
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: 3a521970d749aad5b752bc8cd224455b5854e424
ms.sourcegitcommit: 4665ebce0c106bdb52eef36e544280b496b6f50b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122988167"
---
# <a name="jet_snt"></a>JET_SNT


_**Применимо к:** Windows | Windows Сервером_

## <a name="jet_snt"></a>JET_SNT

[JET_SNT]() группа констант описывает точки выполнения операции, сведения о которой запрашиваются при вызове функции обратного вызова [JET_PFNSTATUS](./jet-pfnstatus-callback-function.md) .


| <p>Константа/значение</p> | <p>Описание</p> | 
|-----------------------|--------------------|
| <p>JET_sntBegin<br />5</p> | <p>Начало операции</p> | 
| <p>JET_sntRequirements<br />7</p> | <p>Не поддерживается.</p><p><strong>сервер Windows 2000:</strong>  Операция запущена. В этом случае последний параметр функции обратного вызова должен быть допустимым указателем на <a href="gg269328(v=exchg.10).md">JET_SNPROG</a> структуру, указывающую общее количество единиц для выполнения.</p> | 
| <p>JET_sntProgress<br />0</p> | <p>Число завершенных единиц и количество единиц, которые еще не были выполнены. Эти сведения возвращаются в элементах структуры <a href="gg269328(v=exchg.10).md">JET_SNPROG</a> .</p> | 
| <p>JET_sntComplete<br />6</p> | <p>Завершение операции.</p> | 
| <p>JET_sntFail<br />3</p> | <p>Сбой операции.</p> | 
| <p>JET_sntRecoveryStep<br />8</p> | <p>Управление восстановлением операции.</p><div class="alert">&gt; [!NOTE]&gt; <P>это значение неприменимо к версиям операционной системы Windows, начиная с Windows 8.</P></div> | 



### <a name="requirements"></a>Требования


| Требование | Применение |
|------------|----------|
| <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | 
| <p><strong>Server</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | 
| <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 



### <a name="see-also"></a>См. также:

[JET_PFNSTATUS](./jet-pfnstatus-callback-function.md)  
[JET_SNP](./jet-snp.md)  
[JET_SNPROG](./jet-snprog-structure.md)
