---
description: создание приложений DirectShow
ms.assetid: 2fbdbe49-0d4d-4dce-afc3-7049c793ace0
title: создание приложений DirectShow
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 56c6ab8a0731e93eece734abd4380b092414ff5f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126891704"
---
# <a name="building-directshow-applications"></a>создание приложений DirectShow

в этом разделе описываются заголовки и библиотеки, необходимые для создания приложений DirectShow.

последние DirectShow заголовки и библиотеки доступны в [Windows SDK](https://msdn.microsoft.com/windows/aa904949.aspx).

## <a name="header-files"></a>Файлы заголовков

все приложения DirectShow используют файл заголовка, показанный в следующей таблице.



| Файл заголовка | Требуется для                 |
|-------------|------------------------------|
| DShow. h     | все DirectShow приложения. |



 

для некоторых интерфейсов DirectShow требуются дополнительные файлы заголовков. Эти требования указаны в справочнике по интерфейсу.

## <a name="library-files"></a>Файлы библиотек

DirectShow использует статические файлы библиотеки, приведенные в следующей таблице.



| Файл библиотеки | Описание                                                                                                                    |
|--------------|--------------------------------------------------------------------------------------------------------------------------------|
| Стрмиидс. lib | Экспортирует идентификаторы классов (CLSID) и идентификаторы интерфейса (идентификаторов IID).                                                           |
| Quartz. lib   | Экспортирует функцию [**амжетеррортекст**](/windows/win32/api/errors/nf-errors-amgeterrortexta) . Если не вызвать эту функцию, эта библиотека не требуется. |



 

Используйте одинаковые lib файлы для сборок отладки и выпуска.

## <a name="filter-base-classes"></a>Фильтровать базовые классы

Windows SDK предоставляет набор классов C++, которые рекомендуются при написании настраиваемого фильтра DirectShow. Эти классы предоставляются в виде образца кода, который можно скомпилировать в статическую библиотеку. дополнительные сведения см. в разделе [DirectShow базовых классов](directshow-base-classes.md).

## <a name="redistributable-dlls"></a>Распространяемые библиотеки DLL

DirectShow приложений, написанных для Windows XP с пакетом обновления 2 (sp2) и более поздних версий, не требуется распространять какие-либо DirectShow библиотеки dll.

для Windows XP с пакетом обновления 1 (SP1) и более ранними версиями, распространяемые DirectShow библиотеки dll доступны в пакете SDK для Microsoft DirectX. Последняя версия этих библиотек DLL — версия 9.0 c. Дальнейшая разработка распространяемых библиотек DLL не планируется. Windows XP с пакетом обновления 2 (SP2) содержит библиотеки DLL версии 9.0 c.

Пакеты редстрибутабле содержат следующие библиотеки DLL:

-   dxnt.cab
    -   amstream.dll
    -   devenum.dll
    -   encapi.dll
    -   ks.sys
    -   ksolay.ax
    -   ksproxy.ax
    -   ksuser.dll
    -   l3codecx.ax
    -   mciqtz32.dll
    -   mpg2splt.ax
    -   msdmo.dll
    -   mskssrv.sys
    -   mspclock.sys
    -   mspqm.sys
    -   mstee.sys
    -   mswebdvd.dll
    -   qasf.dll
    -   qcap.dll
    -   qdv.dll
    -   qdvd.dll
    -   qedit.dll
    -   qedwipes.dll
    -   quartz.dll
    -   stream.sys
    -   swenum.sys
-   bda.cab
    -   bdaplgin.ax
    -   bdasup.sys
    -   ccdecode.sys
    -   ipsink.ax
    -   kstvtune.ax
    -   kswdmcap.ax
    -   ksxbar.ax
    -   mpe.sys
    -   mpeg2data.ax
    -   msdv.sys
    -   msdvbnp.ax
    -   msvidctl.dll
    -   msyuv.dll
    -   nabtsfec.sys
    -   ndisip.sys
    -   psisdecd.dll
    -   psisrndr.ax
    -   slip.sys
    -   streamip.sys
    -   vbisurf.ax
    -   wstcodec.sys
    -   wstdecod.dll

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[создание фильтров DirectShow](building-directshow-filters.md)
</dt> </dl>

 

 
