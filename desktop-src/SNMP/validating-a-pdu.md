---
title: Проверка PDU
description: Если приложение WinSNMP вызывает функцию Снмпсендмсг или Снмпенкодемсг, то реализация Microsoft WinSNMP проверяет допустимость PDU и другие параметры функции.
ms.assetid: 0f5754ff-3688-465b-a1ad-bf7d89d7dbd8
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 420fe01fac150bbebf39e494844bf2797ce0edc73d9339e0148c54faceebe8c9
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119885644"
---
# <a name="validating-a-pdu"></a>Проверка PDU

Если приложение WinSNMP вызывает функцию [**снмпсендмсг**](/windows/desktop/api/Winsnmp/nf-winsnmp-snmpsendmsg) или [**снмпенкодемсг**](/windows/desktop/api/Winsnmp/nf-winsnmp-snmpencodemsg) , то реализация Microsoft WINSNMP проверяет допустимость PDU и другие параметры функции.

Значение одного компонента данных PDU (или поля) может быть допустимым по отдельности, но оно может быть недопустимым в сочетании со значениями других полей. Например, если в качестве значения поля **\_ типа PDU** для PDU используется SNMP- \_ PDU \_ или \_ \_ отклика PDU SNMP, то оба поля **\_ состояния ошибки** и **\_ индекса ошибки** должны быть равны нулю. Любое другое сочетание значений представляет собой недопустимый PDU.

Реализация отклоняет недопустимые PDU и возвращает состояние ошибки СНМПАПИ \_ сбой. Он устанавливает расширенный код ошибки, равный СНМПАПИ \_ PDU \_ .

 

 




