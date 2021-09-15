---
title: Перечисление MSDRM_STATUS (Вмдрмсдк. h)
description: '\_Тип перечисления состояния Msdrm определяет условия состояния для подсистемы DRM.'
ms.assetid: b26600ea-2603-4fca-9408-2d5c88091dcc
keywords:
- Формат Windows Media MSDRM_STATUS перечисления
- Формат Windows Media для перечисления
topic_type:
- apiref
api_name:
- MSDRM_STATUS
api_location:
- Wmdrmsdk.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: bf2a73de9e33216e22a01966be8f2ed6a3185fdf
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572159"
---
# <a name="msdrm_status-enumeration"></a>\_Перечисление состояния Msdrm

Тип **перечисления \_ состояния Msdrm** определяет условия состояния для подсистемы DRM.

## <a name="syntax"></a>Синтаксис


```C++
typedef enum MSDRM_STATUS { 
  DRM_ERROR                        = 0,
  DRM_INFORMATION                  = 1,
  DRM_BACKUPRESTORE_BEGIN          = 2,
  DRM_BACKUPRESTORE_END            = 3,
  DRM_BACKUPRESTORE_CONNECTING     = 4,
  DRM_BACKUPRESTORE_DISCONNECTING  = 5,
  DRM_ERROR_WITHURL                = 6,
  DRM_RESTRICTED_LICENSE           = 7,
  DRM_NEEDS_INDIVIDUALIZATION      = 8,
  DRM_PLAY_OPL_NOTIFICATION        = 9,
  DRM_COPY_OPL_NOTIFICATION        = 10,
  DRM_REFRESHCRL_COMPLETE          = 11
} ;
```



## <a name="constants"></a>Константы

<dl> <dt>

<span id="DRM_ERROR"></span><span id="drm_error"></span>**\_Ошибка DRM**
</dt> <dd>

Указывает, что произошла ошибка.

</dd> <dt>

<span id="DRM_INFORMATION"></span><span id="drm_information"></span>**\_сведения об DRM**
</dt> <dd>

Указывает, что имеются дополнительные сведения о состоянии.

</dd> <dt>

<span id="DRM_BACKUPRESTORE_BEGIN"></span><span id="drm_backuprestore_begin"></span>**\_Начало БАККУПРЕСТОРЕ \_ DRM**
</dt> <dd>

Указывает, что началась операция резервного копирования или восстановления лицензий.

</dd> <dt>

<span id="DRM_BACKUPRESTORE_END"></span><span id="drm_backuprestore_end"></span>**\_конец БАККУПРЕСТОРЕ \_ DRM**
</dt> <dd>

Указывает, что операция резервного копирования или восстановления лицензий завершилась.

</dd> <dt>

<span id="DRM_BACKUPRESTORE_CONNECTING"></span><span id="drm_backuprestore_connecting"></span>**\_Подключение БАККУПРЕСТОРЕ \_ DRM**
</dt> <dd>

Указывает, что выполняется операция резервного копирования или восстановления лицензий и что клиентский компьютер подключается к резервному серверу.

</dd> <dt>

<span id="DRM_BACKUPRESTORE_DISCONNECTING"></span><span id="drm_backuprestore_disconnecting"></span>**Отсоединение DRM \_ баккупресторе \_**
</dt> <dd>

Указывает, что выполняется операция резервного копирования или восстановления лицензий и что клиентский компьютер отключается от резервного сервера.

</dd> <dt>

<span id="DRM_ERROR_WITHURL"></span><span id="drm_error_withurl"></span>**\_Ошибка DRM \_ висурл**
</dt> <dd>

Указывает, что операция DRM обнаружила неверный URL-адрес.

</dd> <dt>

<span id="DRM_RESTRICTED_LICENSE"></span><span id="drm_restricted_license"></span>**\_Лицензия с ограниченными правами DRM \_**
</dt> <dd>

Указывает, что операция DRM не может быть продолжена, так как на клиентском компьютере нет лицензии, предоставляющей требуемое право.

</dd> <dt>

<span id="DRM_NEEDS_INDIVIDUALIZATION"></span><span id="drm_needs_individualization"></span>**DRM \_ требуется \_ индивидуальность**
</dt> <dd>

Указывает, что операция DRM не может быть продолжена, так как подсистема DRM должна быть индивидуальной.

</dd> <dt>

<span id="DRM_PLAY_OPL_NOTIFICATION"></span><span id="drm_play_opl_notification"></span>**\_уведомление DRM Play \_ ОПЛ \_**
</dt> <dd>

Указывает, что операция воспроизведения не может быть завершена, поскольку не выполнены требования к уровню защиты выходных данных.

</dd> <dt>

<span id="DRM_COPY_OPL_NOTIFICATION"></span><span id="drm_copy_opl_notification"></span>**\_ \_ уведомление о копировании ОПЛ DRM \_**
</dt> <dd>

Указывает, что операция копирования не может быть завершена, поскольку не выполнены требования к уровню защиты выходных данных.

</dd> <dt>

<span id="DRM_REFRESHCRL_COMPLETE"></span><span id="drm_refreshcrl_complete"></span>**\_РЕФРЕШКРЛ DRM \_ завершена**
</dt> <dd>

Указывает, что вызов [**ивмдрмсекурити::P ерформсекуритюпдате**](iwmdrmsecurity-performsecurityupdate.md) завершил обновление списка отзыва.

</dd> </dl>

## <a name="remarks"></a>Remarks

Нет.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|---------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмдрмсдк. h</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Типы перечислений**](drm-enumeration-types.md)
</dt> </dl>

 

 





