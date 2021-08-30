---
description: Функции для установки и получения дескриптора безопасности объектов.
ms.assetid: 22bf0d6b-3ec6-4c28-ace4-49e48714f4bf
title: 'Функции дескрипторов безопасности низкого уровня '
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d77c717b554a670eebed4e7df67760fe7e08eb8a
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122470980"
---
# <a name="low-level-security-descriptor-functions"></a>Функции дескрипторов безопасности низкого уровня 

Существует несколько пар низкоуровневых функций для установки и извлечения [*дескриптора безопасности*](/windows/desktop/SecGloss/s-gly)объекта. каждая из этих пар работает только с ограниченным набором объектов Windows. Например, одна пара работает с объектами File, а другая работает с разделами реестра. В следующей таблице показаны низкоуровневые функции для использования с различными типами защищаемых объектов.




| Тип объекта | Низкоуровневые функции | 
|-------------|---------------------|
| <ul><li><a href="/windows/desktop/FileIO/file-security-and-access-rights">Файлы</a></li><li><a href="/windows/desktop/FileIO/file-security-and-access-rights">Directories</a></li><li>маилслотс</li><li><a href="/windows/desktop/ipc/named-pipe-security-and-access-rights">Именованные каналы</a></li></ul> | Используйте функции <a href="/windows/desktop/api/Winbase/nf-winbase-getfilesecuritya"><strong>жетфилесекурити</strong></a> и <a href="/windows/desktop/api/Winbase/nf-winbase-setfilesecuritya"><strong>сетфилесекурити</strong></a> . Эти функции используют символьные строки для обнаружения защищаемого объекта вместо использования дескрипторов. | 
| <ul><li><a href="/windows/desktop/ProcThread/process-security-and-access-rights">Процессы</a></li><li><a href="/windows/desktop/ProcThread/thread-security-and-access-rights">Потоки</a></li><li><a href="access-rights-for-access-token-objects.md">Маркеры доступа в Azure Active Directory</a></li><li><a href="/windows/desktop/Memory/file-mapping-security-and-access-rights">Объекты сопоставления файлов</a></li><li><a href="/windows/desktop/Sync/synchronization-object-security-and-access-rights">Семафоры</a></li><li><a href="/windows/desktop/Sync/synchronization-object-security-and-access-rights">События</a></li><li><a href="/windows/desktop/Sync/synchronization-object-security-and-access-rights">Мьютексы</a></li><li><a href="/windows/desktop/Sync/synchronization-object-security-and-access-rights">Ожидающие таймеры</a></li></ul> | Используйте функции <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-getkernelobjectsecurity"><strong>жеткернелобжектсекурити</strong></a> и <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-setkernelobjectsecurity"><strong>сеткернелобжектсекурити</strong></a> . | 
| <ul><li><a href="/windows/desktop/winstation/window-station-security-and-access-rights">Оконные станции</a></li><li><a href="/windows/desktop/winstation/desktop-security-and-access-rights">Настольные системы</a></li></ul> | Используйте функции <a href="/windows/desktop/api/Winuser/nf-winuser-getuserobjectsecurity"><strong>жетусеробжектсекурити</strong></a> и <a href="/windows/desktop/api/Winuser/nf-winuser-setuserobjectsecurity"><strong>сетусеробжектсекурити</strong></a> . | 
| <ul><li><a href="/windows/desktop/SysInfo/registry-key-security-and-access-rights">Разделы реестра</a></li></ul> | Используйте функции <a href="/windows/desktop/api/Winreg/nf-winreg-reggetkeysecurity"><strong>регжеткэйсекурити</strong></a> и <a href="/windows/desktop/api/Winreg/nf-winreg-regsetkeysecurity"><strong>регсеткэйсекурити</strong></a> . | 
| <ul><li><a href="/windows/desktop/Services/service-security-and-access-rights">Windows объекты службы</a></li></ul> | Используйте функции <a href="/windows/desktop/api/Winsvc/nf-winsvc-queryserviceobjectsecurity"><strong>куерисервицеобжектсекурити</strong></a> и <a href="/windows/desktop/api/Winsvc/nf-winsvc-setserviceobjectsecurity"><strong>сетсервицеобжектсекурити</strong></a> . | 
| <ul><li>Объекты принтера</li></ul> | Используйте структуру <a href="/windows/desktop/printdocs/printer-info-2"><strong>PRINTER_INFO_2</strong></a> с функциями <a href="/windows/desktop/printdocs/getprinter"><strong>PrintOut</strong></a> и <a href="/windows/desktop/printdocs/setprinter"><strong>сетпринтер</strong></a> . | 
| <ul><li><a href="/windows/desktop/NetMgmt/security-requirements-for-the-network-management-functions">Общие сетевые папки</a></li></ul> | Используйте уровень 502 с функциями <a href="/windows/desktop/api/lmshare/nf-lmshare-netsharegetinfo"><strong>нетшарежетинфо</strong></a> и <a href="/windows/desktop/api/lmshare/nf-lmshare-netsharesetinfo"><strong>нетшаресетинфо</strong></a> . | 
| <ul><li><a href="acl-based-access-control.md">Закрытые объекты (объекты являются частными для создания приложения)</a></li></ul> | Используйте функции <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-createprivateobjectsecurity"><strong>креатеприватеобжектсекурити</strong></a>, <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-destroyprivateobjectsecurity"><strong>дестройприватеобжектсекурити</strong></a>, <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-getprivateobjectsecurity"><strong>жетприватеобжектсекурити</strong></a> и <a href="/windows/desktop/api/securitybaseapi/nf-securitybaseapi-setprivateobjectsecurity"><strong>SetPrivateObjectSecurity</strong></a> . | 




 

 

 
