---
title: Узел протокола расширяемой проверки подлинности
description: Сведения о узле протокола расширенной проверки подлинности (EAP). См. требования к времени выполнения и Просмотр дополнительных доступных ресурсов.
ms.assetid: caaef367-2952-44fc-ac4c-f0db6387850e
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 2f007435c43969ad0f195b0a6a1e697ab817d9c4
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127240766"
---
# <a name="extensible-authentication-protocol-host"></a>Узел протокола расширяемой проверки подлинности

## <a name="purpose"></a>Назначение


EAPHost — это компонент сети Microsoft Windows, предоставляющий инфраструктуру протокола EAP для проверки подлинности реализаций протоколов, таких как [802.1 x](/previous-versions/windows/embedded/ms890287(v=msdn.10)) и [точка-точка](https://go.microsoft.com/fwlink/p/?linkid=83919) (PPP). Она также позволяет выполнять проверку подлинности с помощью таких технологий, как сервер политики сети (NPS) (Майкрософт). В отличие от предыдущего сервера IAS ([RADIUS](/windows/desktop/Nps/ias-about-internet-authentication-service)), NPS поддерживает [защиту доступа к сети](/windows/desktop/NAP/network-access-protection-start-page) (NAP).


API-интерфейсы EAPHost позволяют приложениям проходить проверку подлинности с помощью службы EAPHost и предоставлять шаблон для разработки согласованных методов проверки подлинности для использования с EAPHost.

## <a name="run-time-requirements"></a>Требования к среде выполнения

api-интерфейсы EAPHost поддерживаются только в Windows Vista и более поздних операционных системах.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Об EAPHost](about-eap-host.md)
</dt> <dt>

[Использование EAPHost](using-eap-host.md)
</dt> <dt>

[Справочник по API EAPHost](eaphost-api-reference.md)
</dt> </dl>

 

 