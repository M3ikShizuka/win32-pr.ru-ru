---
description: Защита ресурсов предотвращает замену системных файлов и папок и разделов реестра, необходимых операционной системе. Изменение защищенных ресурсов может привести к сбою приложения или системы.
ms.assetid: 27df9300-8bea-4748-9acd-2c1625093ece
title: Windows Защита ресурсов
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b00dabeadc662d3c13923d9d56e442388c53b7fa1e5740c651d689c3098bd049
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120098584"
---
# <a name="windows-resource-protection"></a>Windows Защита ресурсов

## <a name="purpose"></a>Назначение

Windows Защита ресурсов (WRP) предотвращает замену необходимых системных файлов, папок и разделов реестра, которые устанавливаются в составе операционной системы. она стала доступной начиная с Windows Server 2008 и Windows Vista. Приложения не должны перезаписывать эти ресурсы, так как они используются системой и другими приложениями. Защита этих ресурсов предотвращает сбои приложений и операционных систем. WRP — это новое имя для защиты Windows файлов (WFP). WRP защищает разделы и папки реестра, а также ключевые системные файлы.

## <a name="where-applicable"></a>Где применимо

все приложения на основе Windows и программы установки, работающие на Windows Server 2008 или Windows Vista и более поздних операционных системах, должны учитывать WRP. все приложения на основе Windows, работающие на Microsoft Windows Server 2003 или Windows XP, и их программы установки должны знать о WFP.

## <a name="developer-audience"></a>Аудитория разработчиков

API WRP предназначен для использования программистами C/C++. API WRP имеет две функции: [**сфЦисфилепротектед**](/windows/desktop/api/Sfc/nf-sfc-sfcisfileprotected) и [**сфЦискэйпротектед**](/windows/desktop/api/Sfc/nf-sfc-sfciskeyprotected).

## <a name="run-time-requirements"></a>Требования к среде выполнения

для приложений, использующих только функцию [**сфЦисфилепротектед**](/windows/desktop/api/Sfc/nf-sfc-sfcisfileprotected) , требуется Windows server 2008, Windows Vista, Windows Server 2003 или Windows XP. для приложений, использующих функцию [**сфЦискэйпротектед**](/windows/desktop/api/Sfc/nf-sfc-sfciskeyprotected) , требуется Windows Server 2008 или Windows Vista.

## <a name="in-this-section"></a>В этом разделе



| Раздел                                                                                     | Описание                                 |
|-------------------------------------------------------------------------------------------|---------------------------------------------|
| [о защита ресурсов Windows](about-windows-file-protection.md)<br/>         | Общие сведения о WRP.<br/>   |
| [Windows Справочник по защите ресурсов](windows-file-protection-reference.md)<br/> | Справочная документация по WRP.<br/> |



 

 

 




