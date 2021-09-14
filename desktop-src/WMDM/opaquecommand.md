---
title: Структура ОПАКУЕКОММАНД
description: структура опакуекомманд содержит данные для команд, которые передаются на устройство с помощью Windows мультимедиа диспетчер устройств, но не предназначены для обработки Windows Media диспетчер устройств.
ms.assetid: 5b39cf07-2816-4615-a754-e3f0c57bf4ce
keywords:
- Структура ОПАКУЕКОММАНД Windows Media диспетчер устройств
- Структура диспетчер устройств мультимедиа Windows
topic_type:
- apiref
api_name:
- OPAQUECOMMAND
api_location:
- wmdm.idl
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 672147cb99336f95a1ced88a3cc6b8df977aec74
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126967810"
---
# <a name="opaquecommand-structure"></a>Структура ОПАКУЕКОММАНД

структура **опакуекомманд** содержит данные для команд, которые передаются на устройство с помощью Windows мультимедиа диспетчер устройств, но не предназначены для обработки Windows Media диспетчер устройств.

## <a name="syntax"></a>Синтаксис


```C++
typedef struct OPAQUECOMMAND {
  GUID  guidCommand;
  DWORD dwDataLen;
  BYTE  *pData;
  BYTE  abMAC[20];
} ;
```



## <a name="members"></a>Участники

<dl> <dt>

**гуидкомманд**
</dt> <dd>

**Идентификатор GUID** , представляющий запрошенную команду.

</dd> <dt>

**двдатален**
</dt> <dd>

Длина данных, на которые указывает *pData* , в байтах.

</dd> <dt>

**pData**
</dt> <dd>

Данные, необходимые для выполнения команды, и/или данные, возвращаемые командой.

</dd> <dt>

**Абмак \[ 20\]**
</dt> <dd>

Этот код проверки подлинности сообщений (MAC) должен включать в себя элемент **гуидкомманд** , данные, на которые указывает *пдвдатален* , и данные, на которые указывает *pData* , если таковые имеются. Если *pData* имеет **значение NULL**, он не должен включаться в компьютер Mac. ВМДМ \_ Mac \_ length определяется как 20.

</dd> </dl>

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------|-------------------------------------------------------------------------------------|
| Заголовок<br/> | <dl> <dt>Вмдм. idl</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Имдспдевице:: Сендопакуекомманд**](/windows/desktop/api/mswmdm/nf-mswmdm-imdspdevice-sendopaquecommand)
</dt> <dt>

[**Имдспстораже:: Сендопакуекоммандс**](/windows/desktop/api/mswmdm/nf-mswmdm-imdspstorage-sendopaquecommand)
</dt> <dt>

[**Ивмдмдевице:: Сендопакуекомманд**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmdevice-sendopaquecommand)
</dt> <dt>

[**Ивмдмстораже:: Сендопакуекомманд**](/windows/desktop/api/mswmdm/nf-mswmdm-iwmdmstorage-sendopaquecommand)
</dt> <dt>

[**Структуры**](structures.md)
</dt> </dl>

 

 





