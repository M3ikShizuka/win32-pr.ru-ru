---
title: Константы TS_SD_ (Текстстор. h)
description: '\_Константы служб терминалов SD \_ \ описывают динамические состояния документов, используемые приложением во время выполнения.'
ms.assetid: fb673e42-bee7-484e-872a-d709d5ca12f2
topic_type:
- apiref
api_name:
- TS_SD_READONLY
- TS_SD_LOADING
- TS_SD_MASKALL
api_location:
- Textstor.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 565bc97b9fa2d1474f1ba36cd8137e63125541e5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127056740"
---
# <a name="ts_sd_-constants"></a>\_Константы SD служб терминалов \_ \*

Константы SD в службах терминалов \_ \_ \* описывают динамические состояния документов, используемые приложением во время выполнения.



| Константа/значение                                                                                                                                                                                                                                              | Описание                                                  |
|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------------------------------------------------|
| <span id="TS_SD_READONLY"></span><span id="ts_sd_readonly"></span><dl> <dt>**TS \_ SD \_ ReadOnly**</dt> <dt>(0x1)</dt> </dl>                              | Документ доступен только для чтения и не может быть изменен.<br/> |
| <span id="TS_SD_LOADING"></span><span id="ts_sd_loading"></span><dl> <dt>**TS \_ \_Загрузка SD**</dt> <dt>(0x2)</dt> </dl>                                 | Документ загружается и может быть неполным.<br/>  |
| <span id="TS_SD_MASKALL"></span><span id="ts_sd_maskall"></span><dl> <dt>**TS \_ SD \_ Маскалл**</dt> <dt>(TS \_ SD \_ только \| для \_ загрузки SD TS \_ )</dt> </dl> | Документ доступен только для чтения и загружается.<br/>       |



## <a name="remarks"></a>Комментарии

Элемент **двдинамикфлагс** структуры [ \_ состояния служб терминалов](/windows/desktop/api/Textstor/ns-textstor-ts_status) использует эти константы.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                              |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                    |
| Распространяемые компоненты<br/>          | TSF 1,0 на Windows 2000 Professional<br/>                                         |
| Заголовок<br/>                   | <dl> <dt>Текстстор. h</dt> </dl>   |
| IDL<br/>                      | <dl> <dt>Текстстор. idl</dt> </dl> |



## <a name="see-also"></a>См. также:

<dl> <dt>

[\_состояние TS](/windows/desktop/api/Textstor/ns-textstor-ts_status)
</dt> <dt>

[\_ \_ \* Константы TF SD](tf-sd--constants.md)
</dt> </dl>

 

 





