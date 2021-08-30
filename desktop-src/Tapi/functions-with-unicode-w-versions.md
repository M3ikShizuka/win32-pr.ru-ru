---
description: Дополнительные сведения см. в статье функции с версиями в Юникоде (W)
ms.assetid: 3457cfb6-3891-4e15-a4e0-53ad43adcc2d
title: Функции с версиями в Юникоде (W)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1ff46188554c54c19e80f80fd723500f08077a40
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122469571"
---
# <a name="functions-with-unicode-w-versions"></a>Функции с версиями в Юникоде (W)

Следующие функции TAPI реализуются в версиях Юникод (W) и ANSI (A). Как правило, реализация версии ANSI вызывает версию Юникода и выполняет необходимые преобразования параметров ANSI и полей структуры в Юникод и обратно. в следующей таблице указаны параметры, которые преобразуются.

Для совместимости с предыдущими версиями TAPI приложения, явно вызывающие универсальный (ни "W", ни "A") версию функции, будут выполнять версию ANSI.

> [!Note]  
> Весь интерфейс поставщика услуг телефонии (ТСПИ) — это Юникод для версии 2,0.

 

В следующей таблице приведены ссылки на строковые поля в структурах TAPI, состоящие из части имен полей. Например, "адрес вызывающего объекта" в структуре [**линефорвард**](/windows/desktop/api/Tapi/ns-tapi-lineforward) указывает поле **двкаллераддрессоффсет** и отделяется полем **двкаллераддресссизе** . в таблице эта строка определяется просто как **каллераддресс**.




| Функция TAPI | Параметры и поля структуры, преобразованные в версии функции ANSI | 
|---------------|-----------------------------------------------------------------------|
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineaddprovider"><strong>линеаддпровидер</strong></a> | <em>лпсзпровидернаме</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineblindtransfer"><strong>линеблиндтрансфер</strong></a> | <em>лпсздестаддресс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineconfigdialog"><strong>линеконфигдиалог</strong></a> | <em>лпсздевицекласс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineconfigdialogedit"><strong>линеконфигдиаложедит</strong></a> | <em>лпсздевицекласс</em><blockquote>[!Note]<br />Приложение должно обрабатывать преобразование строк в <em>лпдевицеконфигин</em> и <em>лпдевицеконфигаут</em>, если они управляются напрямую.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linedial"><strong>линедиал</strong></a> | <em>лпсздестаддресс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineforward"><strong>линефорвард</strong></a> | <em>лпфорвардлист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineforwardlist"><strong>линефорвардлист</strong></a>)<ul><li><em>Форвардлист</em> ( <a href="/windows/desktop/api/Tapi/ns-tapi-lineforward"><strong>линефорвард</strong></a>)<ul><li><em>каллераддресс</em></li><li><em>дестаддресс</em></li></ul></li></ul><em>лпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<br /><ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegatherdigits"><strong>линегасердигитс</strong></a> | <em>лпсдигитслпсзтерминатиондигитс</em><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegeneratedigits"><strong>линеженератедигитс</strong></a> | <em>лпсздигитс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetaddresscaps"><strong>линежетаддресскапс</strong></a> | <em>лпаддресскапс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineaddresscaps"><strong>линеаддресскапс</strong></a>)<ul><li><em>Адрес</em></li><li><em>комплетионмсгтекст</em></li><li><em>девицеклассес</em></li><li><em>Каллтреатментлист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecalltreatmententry"><strong>линекаллтреатментентри</strong></a>)</li><li><em>каллтреатментнаме</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetaddressid"><strong>линежетаддрессид</strong></a> | <em>лпсаддресс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetaddressstatus"><strong>линежетаддрессстатус</strong></a> | <em>лпаддрессстатус</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineaddressstatus"><strong>линеаддрессстатус</strong></a>)<ul><li><em>Вперед</em> ( <a href="/windows/desktop/api/Tapi/ns-tapi-lineforward"><strong>линефорвард</strong></a>)</li><li><em>каллераддресс</em></li><li><em>дестаддресс</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetagentactivitylista"><strong>линежетажентактивитилист</strong></a> | <em>лпажентактивитилист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentactivitylist"><strong>линеажентактивитилист</strong></a>)<ul><li><em>Список</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentactivityentry"><strong>линеажентактивитентри</strong></a>)</li><li><em>имя</em>;</li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetagentcapsa"><strong>линежетаженткапс</strong></a> | <em>лпаженткапс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentcaps"><strong>линеаженткапс</strong></a>)<ul><li><em>аженсандлеринфо</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetagentgrouplista"><strong>линежетажентграуплист</strong></a> | <em>лпажентграуплисти</em>( <a href="/windows/win32/api/tapi/ns-tapi-lineagentgrouplist"><strong>линеажентграуплист</strong></a>)<ul><li><em>Список</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentgroupentry"><strong>линеажентграупентри</strong></a>)</li><li><em>имя</em>;</li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetagentstatusa"><strong>линежетажентстатус</strong></a> | <em>лпажентстатус</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentstatus"><strong>линеажентстатус</strong></a>)<ul><li><em>Действие</em></li><li><em>Грауплист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineagentgroupentry"><strong>линеажентграупентри</strong></a>)</li><li><em>имя</em>;</li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetapppriority"><strong>линежетаппприорити</strong></a> | <em>лпсзаппфиленамелпекстенсионнаме</em><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetcallinfo"><strong>линежеткаллинфо</strong></a> | <em>лпкаллинфо</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallinfo"><strong>линекаллинфо</strong></a>)<ul><li><em>каллерид</em></li><li><em>каллериднаме</em></li><li><em>калледид</em></li><li><em>калледиднаме</em></li><li><em>коннектид</em></li><li><em>коннектедиднаме</em></li><li><em>редиректионид</em></li><li><em>редиректиониднаме</em></li><li><em>редиректингид</em></li><li><em>редиректингиднаме</em></li><li><em>AppName</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetcountry"><strong>линежеткаунтри</strong></a> | <em>лплинекаунтрилист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecountrylist"><strong>линекаунтрилист</strong></a>)<ul><li><em>Каунтрилист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecountryentry"><strong>линекаунтрентри</strong></a>)</li><li><em>CountryName</em></li><li><em>самеареаруле</em></li><li><em>лонгдистанцеруле</em></li><li><em>интернатионалруле</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetdevcaps"><strong>линежетдевкапс</strong></a> | <em>лплинедевкапс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linedevcaps"><strong>линедевкапс</strong></a>)<ul><li><em>провидеринфо</em></li><li><em>свитчинфо</em></li><li><em>линенаме</em></li><li><em>терминалтекст</em></li><li><em>девицеклассес</em></li></ul><blockquote>[!Note]<br /><em>двстрингформат</em> устарел.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetdevconfig"><strong>линежетдевконфиг</strong></a> | <em>лпсздевицекласс</em><blockquote>[!Note]<br />Приложение должно обрабатывать преобразование строк в <em>лпдевицеконфиг</em>, если они напрямую управляются.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegeticon"><strong>линежетикон</strong></a> | <em>лпсздевицекласс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetid"><strong>линежетид</strong></a> | <em>лпсздевицекласс</em><blockquote>[!Note]<br />Приложение должно обрабатывать преобразование строк в <em>лпдевицеид</em>, если они напрямую управляются.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetlinedevstatus"><strong>линежетлинедевстатус</strong></a> | <em>лплинедевстатус</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linedevstatus"><strong>линедевстатус</strong></a>)<ul><li><em>AppInfo</em> (линеаппинфо)</li><li><em>MachineName</em></li><li><em>UserName</em></li><li><em>модулефиленаме</em></li><li><em>FriendlyName</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetproviderlist"><strong>линежетпровидерлист</strong></a> | <em>лппровидерлист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineproviderlist"><strong>линепровидерлист</strong></a>)<ul><li><em>Провидерлист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-lineproviderentry"><strong>линепровидерентри</strong></a>)</li><li><em>провидерфиленаме</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegetrequest"><strong>линежетрекуест</strong></a> | <em>лпрекуестбуффер</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linereqmakecall"> <strong>линерекмакекалл</strong></a><ul><li><em>сздестаддресс</em></li><li><em>сзаппнаме</em></li><li><em>сзкалледпарти</em></li><li><em>сзкоммент</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linegettranslatecaps"><strong>линежеттранслатекапс</strong></a> | <em>лптранслатекапс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linetranslatecaps"><strong>линетранслатекапс</strong></a>)<ul><li><em>Кардлист</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecardentry"><strong>линекардентри</strong></a>)</li><li><em>CardName</em></li><li><em>самеареаруле</em></li><li><em>лонгдистанцеруле</em></li><li><em>интернатионалруле</em></li><li><em>LocationList</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linelocationentry"> <strong>линелокатионентри</strong></a></li><li><em>LocationName</em></li><li><em>Цитикоде</em></li><li><em>локалакцесскоде</em></li><li><em>лонгдистанцеакцесскоде</em></li><li><em>толлпрефикслист</em></li><li><em>целкаллваитинг</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linehandoff"><strong>линехандофф</strong></a> | <em>лпсзфиленаме</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineinitializeexa"><strong>линеинитиализикс</strong></a> | <em>лпсзфриендляппнаме</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linemakecall"><strong>линемакекалл</strong></a> | <em>лпсздестаддресслпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<br /><ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineopen"><strong>линеопен</strong></a> | <em>лпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linepark"><strong>линепарк</strong></a> | <em>лпсздираддресслпнондираддресс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-varstring"><strong>варстринг</strong></a>)<br /><ul><li><em>String</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linepickup"><strong>линепиккуп</strong></a> | <em>лпсздестаддресслпсзграупид</em><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineprepareaddtoconference"><strong>линепрепареаддтоконференце</strong></a> | <em>лпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineredirect"><strong>линередирект</strong></a> | <em>лпсздестаддресс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linesetapppriority"><strong>линесетаппприорити</strong></a> | <em>лпсзаппфиленамелпсзекстенсионнаме</em><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linesetdevconfig"><strong>линесетдевконфиг</strong></a> | <em>лпсздевицекласс</em><blockquote>[!Note]<br />Приложение должно обрабатывать преобразование строк в <em>лпдевицеконфиг</em>, если они напрямую управляются.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linesettolllist"><strong>линесеттолллист</strong></a> | <em>лпсзаддрессин</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linesetupconference"><strong>линесетупконференце</strong></a> | <em>лпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linesetuptransfer"><strong>линесетуптрансфер</strong></a> | <em>лпкаллпарамс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linecallparams"><strong>линекаллпарамс</strong></a>)<ul><li><em>оригаддресс</em></li><li><em>дисплайаблеаддресс</em></li><li><em>калледпарти</em></li><li><em>Комментарий</em></li><li><em>TargetAddress</em></li><li><em>DeviceClass</em></li><li><em>каллингпартид</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linetranslateaddress"><strong>линетранслатеаддресс</strong></a> | <em>лпсзаддрессинлптранслатеаутпут</em> ( <a href="/windows/win32/api/tapi/ns-tapi-linetranslateoutput"><strong>линетранслатеаутпут</strong></a>)<br /><ul><li><em>диалаблестринг</em></li><li><em>дисплайаблестринг</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-linetranslatedialog"><strong>линетранслатедиалог</strong></a> | <em>лпсзаддрессин</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-lineunpark"><strong>линеунпарк</strong></a> | <em>лпсздестаддресс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phoneconfigdialog"><strong>фонеконфигдиалог</strong></a> | <em>лпсздевицекласс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonegetbuttoninfo"><strong>фонежетбуттонинфо</strong></a> | <em>лпбуттонинфо</em> ( <a href="/windows/win32/api/tapi/ns-tapi-phonebuttoninfo"><strong>фонебуттонинфо</strong></a>)<ul><li><em>ButtonText</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonegetdevcaps"><strong>фонежетдевкапс</strong></a> | <em>лпфонекапс</em> ( <a href="/windows/win32/api/tapi/ns-tapi-phonecaps"><strong>фонекапс</strong></a>)<ul><li><em>провидеринфо</em></li><li><em>фонеинфо</em></li><li><em>фоненаме</em></li><li><em>классы устройств;</em></li></ul><blockquote>[!Note]<br /><em>двстрингформат</em> устарел.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonegeticon"><strong>фонежетикон</strong></a> | <em>лпсздевицекласс</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonegetid"><strong>фонежетид</strong></a> | <em>лпсздевицекласс</em><blockquote>[!Note]<br />Приложение должно обрабатывать преобразование строк в <em>лпдевицеид</em>, если они напрямую управляются.</blockquote><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonegetstatus"><strong>фонежетстатус</strong></a> | <em>лпфонестатус</em> ( <a href="/windows/win32/api/tapi/ns-tapi-phonestatus"><strong>фонестатус</strong></a>)<ul><li><em>OwnerName</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phoneinitializeexa"><strong>фонеинитиализикс</strong></a> | <em>лпсзфриендляппнаме</em> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-phonesetbuttoninfo"><strong>фонесетбуттонинфо</strong></a> | <em>лпбуттонинфо</em> ( <a href="/windows/win32/api/tapi/ns-tapi-phonebuttoninfo"><strong>фонебуттонинфо</strong></a>)<ul><li><em>буттонтест</em></li></ul> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-tapigetlocationinfo"><strong>тапижетлокатионинфо</strong></a> | <em>лпсзкаунтрикоделпсзЦитикоде</em><br /> | 
| <a href="/windows/desktop/api/Tapi/nf-tapi-tapirequestmakecall"><strong>тапирекуестмакекалл</strong></a> | <em>лпсздестаддресслпсзаппнаме</em><br /><em>лпсзкалледпарти</em><br /><em>лпсзкоммент</em><br /> | 




 

 

 




