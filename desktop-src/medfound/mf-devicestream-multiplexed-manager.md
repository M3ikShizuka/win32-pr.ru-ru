---
description: Предоставляет экземпляр Имфмуксстреаматтрибутесманажер, который управляет Имфаттрибутес, описывающим подпотоки мультиплексированного источника мультимедиа.
ms.assetid: 0149BD8B-8C9D-47FD-9EC1-BEBEE73BC73E
title: Атрибут MF_DEVICESTREAM_MULTIPLEXED_MANAGER (Мфидл. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 4b2c022f2bb74756ce1a6afe471c23911c90a208e2940e9919f275df10a78ff1
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119956664"
---
# <a name="mf_devicestream_multiplexed_manager-attribute"></a>\_Атрибут девицестреам \_ мультиплексированного \_ диспетчера MF

Предоставляет экземпляр [**имфмуксстреаматтрибутесманажер**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmuxstreamattributesmanager) , который управляет [**имфаттрибутес**](/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes) , описывающим подпотоки мультиплексированного источника мультимедиа.

## <a name="data-type"></a>Тип данных

**[**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown)**

## <a name="remarks"></a>Remarks

Передайте это значение в [**имфаттрибутес:: Ununknown**](/windows/desktop/api/mfobjects/nf-mfobjects-imfattributes-getunknown) , чтобы определить, предоставляет ли источник мультимедиа мультиплексированные потоки, и, если это так, получите экземпляр [**имфмуксстреаматтрибутесманажер**](/windows/desktop/api/mfobjects/nn-mfobjects-imfmuxstreamattributesmanager).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10, только для \[ настольных приложений версии 1703\]<br/>                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                          |
| Заголовок<br/>                   | <dl> <dt>Мфидл. h</dt> </dl> |



 

 
