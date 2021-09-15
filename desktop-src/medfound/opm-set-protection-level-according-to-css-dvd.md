---
description: Задает уровень защиты HDCP для воспроизведения DVD-дисков, следующие правила системы расшифровки содержимого DVD-диска (CSS).
ms.assetid: 8d9ecb9b-8528-4b23-ab2f-234ba2cb7ed0
title: OPM_SET_PROTECTION_LEVEL_ACCORDING_TO_CSS_DVD (Опмапи. h)
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 971d288367bdc5c59e11bdfd5b86fb233755c95e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574819"
---
# <a name="opm_set_protection_level_according_to_css_dvd"></a>ОПМ \_ установить \_ \_ уровень защиты \_ в \_ соответствии \_ с \_ DVD-диском CSS

Задает уровень защиты HDCP для воспроизведения DVD-дисков, следующие правила системы расшифровки содержимого DVD-диска (CSS).



| Требование | Значение |
|--------------|-----------------------------------------------------------------------------------------------------|
| Идентификатор GUID команды | ОПМ \_ установить \_ \_ уровень защиты \_ в \_ соответствии \_ с \_ DVD-диском CSS                                                |
| Входные данные   | Структура [**\_ \_ \_ \_ параметров уровня защиты ОПМ Set**](/windows/desktop/api/opmapi/ns-opmapi-opm_set_protection_level_parameters) |



 

## <a name="remarks"></a>Комментарии

Эта команда используется для установки High-Bandwidth Digital Защита содержимого (HDCP) при воспроизведении стандартных DVD-дисков. В отличие от команды [**ОПМ \_ Set \_ Protection \_ Level**](opm-set-protection-level.md) , если HDCP не может быть задан по какой либо причине, эта команда не останавливает воспроизведение. (Правила CSS для DVD-дисков содержат «лучшие усилия» для игроков.) В противном случае эта команда идентична команде **ОПМ \_ Set \_ Protection \_ Level** .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения Vista\]<br/>                                      |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2008\]<br/>                                |
| Заголовок<br/>                   | <dl> <dt>Опмапи. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Иопмвидеуутпут:: Configure**](/windows/desktop/api/opmapi/nf-opmapi-iopmvideooutput-configure)
</dt> <dt>

[Команды ОПМ](opm-commands.md)
</dt> </dl>

 

 




