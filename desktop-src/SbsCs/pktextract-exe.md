---
description: Pktextract.exe — это средство, которое извлекает атрибут publicKeyToken из файла сертификата.
ms.assetid: 195ff5bd-bb60-4053-9308-ceacd29853c0
title: Pktextract.exe
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bd163efabd01d65969788aefc2386b2f49079729
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064801"
---
# <a name="pktextractexe"></a>Pktextract.exe

Pktextract.exe — это средство, которое извлекает атрибут **PublicKeyToken** из файла сертификата. Выходные данные — это **PublicKeyToken**, который представляет собой уникальный 16-символьный (8-байтовый) идентификатор открытого ключа, присутствующего в сертификате, в формате, который можно легко вставлять в инструкцию Identity. Файл сертификата должен находиться в том же каталоге, что и Pktextract.exe для использования программы. Pktextract.exe предоставляется в пакете Microsoft Windows Software Development Kit (SDK).

## <a name="syntax"></a>Синтаксис

**pktextract.exe** *<имя_файла. cer>* **\[ -quiet \] \[ -Logo \]**

## <a name="command-line-options"></a>Параметры командной строки

В Pktextract.exe используются следующие параметры командной строки без учета регистра.



| Параметр  | Описание                                                          |
|---------|----------------------------------------------------------------------|
| -quiet  | Подавляет полный вывод сведений о сертификате. Необязательный параметр.        |
| -nologo | Выполняется без отображения стандартных данных об авторских правах Майкрософт. Необязательный элемент. |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Средства разработки параллельных сборок](side-by-side-assembly-development-tools.md)
</dt> </dl>

 

 



