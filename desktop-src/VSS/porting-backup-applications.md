---
description: двоичные файлы из Windows server 2003 с пакетом обновления 1 (SP1) совместимы с Windows Vista и Windows Server 2008. однако двоичные файлы из более ранних версий Windows должны быть перекомпилированы.
ms.assetid: ef40fdf6-b039-4664-bafb-b88c9286c010
title: Перенос приложений резервного копирования
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b85f052996e2c82b11f545bb604b0ed50a886420
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461318"
---
# <a name="porting-backup-applications"></a>Перенос приложений резервного копирования

двоичные файлы из Windows server 2003 с пакетом обновления 1 (SP1) совместимы с Windows Vista и Windows Server 2008. однако двоичные файлы из более ранних версий Windows должны быть перекомпилированы.

## <a name="porting-windows-xp-backup-applications-to-windows-vista"></a>перенос приложений резервного копирования Windows XP в Windows Vista

с момента Windows XP изменилось несколько интерфейсов VSS. как минимум, приложения Windows XP должны быть перекомпилированы с помощью файлов заголовков и библиотек из пакета sdk для VSS 7,2 или пакета sdk для Windows Vista или Windows Server 2008.

## <a name="porting-windows-server-2003-sp1-backup-applications-to-windows-vista"></a>перенос приложений резервного копирования Windows Server 2003 с пакетом обновления 1 (SP1) в Windows Vista

двоичные файлы из Windows server 2003 с пакетом обновления 1 (SP1) совместимы с Windows Vista и Windows Server 2008. однако большинство приложений Windows Server 2003 с пакетом обновления 1 (SP1) необходимо обновить для учета новых функций, которые описаны в следующих разделах.

## <a name="compiling-backup-applications-for-windows-vista"></a>компиляция приложений резервного копирования для Windows Vista

приложения, использующие интерфейсы, доступные в Windows Server 2003, могут быть скомпилированы с помощью файлов заголовков и библиотек, предоставленных в пакете SDK для VSS 7,2. для использования новых интерфейсов приложения должны быть перекомпилированы с помощью файлов заголовков и библиотек, входящих в состав пакета SDK для Windows Vista.

> [!Note]  
> двоичные файлы, скомпилированные с помощью Windows Vista или Windows server 2008, несовместимы с Windows Server 2003 с пакетом обновления 1 (SP1) или более ранними версиями Windows.

 

 

 



