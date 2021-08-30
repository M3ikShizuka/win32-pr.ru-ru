---
description: Определяет элементы конфигурации 802.1 X.
ms.assetid: 4755356e-cb4b-4eed-a494-ca0d17f5184f
title: Схема OneX
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: bb0dc7dd9f8e7561795479de774bf01464cf897800a974df234738aab4a659f7
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119800714"
---
# <a name="onex-schema"></a>Схема OneX

Схема OneX определяет элементы конфигурации 802.1 X. Все элементы схемы OneX применяются к профилям проводного и беспроводного подключения. Список определенных элементов см. в разделе [элементы схемы OneX](onexschema-elements.md).

Корневым элементом профиля 802.1 X является элемент [**OneX**](onexschema-onex-element.md) . Каждый профиль будет иметь только один корневой элемент. Элемент **OneX** находится в `https://www.microsoft.com/networking/OneX/v1` пространстве имен.

Чтобы просмотреть образцы профилей для беспроводных сетей, включающих элементы конфигурации 802.1 X, см. следующие примеры профилей:

-   [Образец профиля начальной загрузки](bootstrap-profile-sample.md)
-   [Пример профиля FIPS](fips-profile-sample.md)
-   [Пример профиля с одним Sign-On](single-sign-on-profile-sample.md)
-   [пример профиля WPA-Enterprise с PEAP-MSCHAPv2](wpa-enterprise-with-peap-mschapv2-profile-sample.md)
-   [пример профиля WPA-Enterprise с TLS](wpa-enterprise-with-tls-profile-sample.md)
-   [пример профиля WPA2-Enterprise с PEAP-MSCHAPv2](wpa2-enterprise-with-peap-mschapv2-profile-sample.md)
-   [пример профиля WPA2-Enterprise с TLS](wpa2-enterprise-with-tls-profile-sample.md)

Чтобы просмотреть образцы профилей для проводных сетей, содержащих элементы конфигурации 802.1 X, см. следующие примеры профилей:

-   [Пример профиля сертификата компьютера](machine-certificate-profile-sample.md)
-   [Пример профиля PEAP](peap-profile-sample.md)
-   [Пример профиля сертификата смарт-карты](smart-card-certificate-profile-sample.md)

 

 



