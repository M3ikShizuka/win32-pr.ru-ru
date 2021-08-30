---
description: Для экспорта и импорта сведений о открытом ключе Диффи-Хелмана используются открытые ключи BLOB-объектов DSS версии 3 типа ПУБЛИККЭЙБЛОБ.
ms.assetid: 9aac1d61-8b61-4f0f-b037-afe4a60302de
title: BLOB-объекты открытого ключа DSS версии 3
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 077aa9bb10569fac60d965ee6d5938984f3d579c
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122473420"
---
# <a name="dss-version-3-public-key-blobs"></a>BLOB-объекты открытого ключа DSS версии 3

Для экспорта и импорта сведений о открытом ключе Диффи-Хелмана используются [*открытые ключи BLOB-объектов*](../secgloss/p-gly.md) DSS версии 3 типа публиккэйблоб. Они имеют следующий формат:


```C++
BLOBHEADER blobheader; 
        // As explained under "Data Structures"
DSSPUBKEY_VER3 dsspubkeyver3;
BYTE p[dsspubkeyver3.bitlenP/8]; 
       // Where P is the prime modulus
BYTE q[dsspubkeyver3.bitlenQ/8]; 
       // Where Q is a large factor of P-1
BYTE g[dsspubkeyver3.bitlenP/8]; 
       // Where G is the generator parameter
BYTE j[dsspubkeyver3.bitlenJ/8]; 
       // Where J is (P-1)/Q
BYTE y[dsspubkeyver3.bitlenP/8]; 
       // Where Y is (G^X) mod P
```



Этот формат [*большого двоичного объекта*](../secgloss/b-gly.md) экспортируется, когда \_ флаг шифрования BLOB \_ -объекта VER3 используется с [**криптекспорткэй**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptexportkey). Так как версия находится в большом двоичном объекте, нет необходимости указывать флаг при использовании этого большого двоичного объекта с [**криптимпорткэй**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptimportkey).

Кроме того, этот формат больших двоичных объектов используется с функцией [**криптсеткэйпарам**](/windows/desktop/api/Wincrypt/nf-wincrypt-cryptsetkeyparam) , если параметр *двпарам* значение параметра \_ Pub \_ используется для задания параметров ключа в DSS-ключе. Это делается, если \_ для создания ключа использовался флаг шифрования прежен. При использовании в этой ситуации значение y игнорируется и поэтому не должно включаться в большой двоичный объект.

В следующей таблице описаны все компоненты большого двоичного объекта ключа.




| Поле | Описание | 
|-------|-------------|
| блобхеадер | Структура <a href="/windows/desktop/api/Wincrypt/ns-wincrypt-publickeystruc"><strong>блобхеадер</strong></a> . Элемент <strong>бтипе</strong> должен иметь значение публиккэйблоб. | 
| Dsspubkeyver3 | Структура <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a> . Для элемента <strong>Magic</strong> необходимо задать значение "DSS3" (0x33535344) для открытых ключей. Обратите внимание, что шестнадцатеричное значение — это просто кодировка <a href="/windows/desktop/SecGloss/a-gly"><em>ASCII</em></a> "DSS3".<br /> | 
| P | Значение P размещается непосредственно после структуры <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a> и всегда должно быть длиной в байтах поля DSSPUBKEY_VER3 <strong>битленп</strong> (разрядная длина P), разделенного на 8 (формат с<a href="/windows/desktop/SecGloss/l-gly"><em>прямым порядком байтов</em></a> ). | 
| Q | Значение Q находится непосредственно после значения P и всегда должно быть длиной в байтах <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a>элемента<strong>битленк</strong> , разделенного на восемь (формат с<a href="/windows/desktop/SecGloss/l-gly"><em>прямым порядком байтов</em></a> ). | 
| G | Значение G расположено непосредственно после значения Q и всегда должно быть длиной в байтах <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a>элемента<strong>битленп</strong> (разрядность P), разделенного на восемь. Если длина данных равна одному или нескольким байтам, меньшим, чем P, деленному на 8, то данные должны быть дополнены требуемыми байтами (нулевыми значениями), чтобы данные были требуемой длины (формат с<a href="/windows/desktop/SecGloss/l-gly"><em>прямым порядком байтов</em></a> ). | 
| J | Значение J расположено непосредственно после значения G и всегда должно быть длиной в байтах <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a>элемента<strong>битленж</strong> , разделенного на восемь (формат с<a href="/windows/desktop/SecGloss/l-gly"><em>прямым порядком байтов</em></a> ). Если значение Битленк равно 0, то это значение отсутствует в большом двоичном объекте. | 
| Да | Значение Y (G ^ X) mod P находится непосредственно после значения J и всегда должно быть длиной (в байтах) <a href="/previous-versions/windows/desktop/legacy/aa381983(v=vs.85)"><strong>DSSPUBKEY_VER3</strong></a>элемента<strong>Битленп</strong> (длина P), деленная на восемь. Если длина данных, полученная в результате вычисления (G ^ X) mod P, равна одному или более байтам, меньшим, чем P, то данные должны быть дополнены требуемыми байтами (нулевыми значениями), чтобы данные были требуемой длины (формат с<a href="/windows/desktop/SecGloss/l-gly"><em>прямым порядком байтов</em></a> ).<blockquote>[!Note]<br />Если эта структура используется с <a href="/windows/desktop/api/Wincrypt/nf-wincrypt-cryptsetkeyparam"><strong>криптсеткэйпарам</strong></a> со значением <em>двпарам</em> KP_PUB_PARAMS, то это значение не включается в большой двоичный объект.</blockquote><br /><br /> | 




 

> [!Note]  
> Большие двоичные объекты с открытым ключом не шифруются, но содержат открытые ключи в виде обычного текста.

 

 

 
