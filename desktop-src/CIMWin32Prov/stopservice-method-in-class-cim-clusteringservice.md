---
description: Останавливает службу, представленную объектом, производным от CIM \_ клустерингсервице.
ms.assetid: b8dbaeeb-819b-469b-9f5e-d658e88d1a6e
ms.tgt_platform: multiple
title: Метод «начало» класса CIM_ClusteringService (Сдоиас. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_ClusteringService.StopService
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: a3a55f7b0a9527092e51156d55c7513ee59c4861
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127054828"
---
# <a name="stopservice-method-of-the-cim_clusteringservice-class"></a>Метод «начало» \_ класса CIM клустерингсервице

Метод **«** незавершенный» останавливает службу, представленную объектом, производным от [**CIM \_ клустерингсервице**](cim-clusteringservice.md). Этот метод наследуется [**от \_ службы CIM**](cim-service.md).

> [!IMPORTANT]
> Классы CIM (модель CIM) в DMTF (распределенная задача управления) являются родительскими классами, на которых строятся классы WMI. В настоящее время WMI поддерживает только [схемы версии CIM 2. x](https://dmtf.org/standards/cim/schemas).

 

В этом разделе используется синтаксис MOF-файл (MOF). Дополнительные сведения об использовании этого метода см. [в разделе вызов метода](/windows/desktop/WmiSdk/calling-a-method).

## <a name="syntax"></a>Синтаксис


```mof
uint32 StopService();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение 0 (нуль), если служба была успешно остановлена, 1 (один), если запрос не поддерживается, и любое другое число для указания ошибки.

## <a name="remarks"></a>Комментарии

В настоящее время этот метод не реализован инструментарием WMI. Чтобы использовать этот метод, его необходимо реализовать в собственном поставщике.

Эта документация является производной от описаний класса CIM, опубликованных в формате DMTF. Корпорация Майкрософт могла внести изменения в Исправление незначительных ошибок, соответствовать стандартам документации пакета Microsoft SDK или предоставить дополнительные сведения.

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| Заголовок<br/>                   | <dl> <dt>Сдоиас. h</dt> </dl>     |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**\_КЛУСТЕРИНГСЕРВИЦЕ CIM**](stopservice-method-in-class-cim-clusteringservice.md)
</dt> <dt>

[**\_КЛУСТЕРИНГСЕРВИЦЕ CIM**](cim-clusteringservice.md)
</dt> </dl>

 

