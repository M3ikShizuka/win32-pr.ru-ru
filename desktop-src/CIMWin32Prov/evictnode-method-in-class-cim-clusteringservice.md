---
description: Метод Евиктноде удаляет компьютерную систему из кластера. Удаляемый узел указывается в качестве параметра метода.
ms.assetid: 4691d536-ade3-4a02-bc28-e31ebaf5d9e4
ms.tgt_platform: multiple
title: Метод Евиктноде класса CIM_ClusteringService
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CIM_ClusteringService.EvictNode
api_type:
- COM
api_location:
- CIMWin32.dll
ms.openlocfilehash: f5574548781f4ab5b7ecbc1ead08aba10ec0bfaf8c0740e2e429303732e90e88
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120077654"
---
# <a name="evictnode-method-of-the-cim_clusteringservice-class"></a>Метод Евиктноде \_ класса CIM клустерингсервице

Метод **евиктноде** удаляет компьютерную систему из кластера. Удаляемый узел указывается в качестве параметра метода.

> [!IMPORTANT]
> Классы CIM (модель CIM) в DMTF (распределенная задача управления) являются родительскими классами, на которых строятся классы WMI. В настоящее время WMI поддерживает только [схемы версии CIM 2. x](https://dmtf.org/standards/cim/schemas).

 

В этом разделе используется синтаксис MOF-файл (MOF). Дополнительные сведения об использовании этого метода см. [в разделе вызов метода](/windows/desktop/WmiSdk/calling-a-method).

## <a name="syntax"></a>Синтаксис


```mof
uint32 EvictNode(
  [in] CIM_ComputerSystem REF CS
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*CS* \[ окне\]
</dt> <dd>

Ссылка на компьютерную систему, которую необходимо удалить из кластера.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает 0 (нуль), если компьютерная система успешно удалена, 1 (один), если метод не поддерживается, и любое другое число, если произошла ошибка.

## <a name="remarks"></a>Remarks

В настоящее время этот метод не реализован инструментарием WMI. Чтобы использовать этот метод, его необходимо реализовать в собственном поставщике.

Эта документация является производной от описаний класса CIM, опубликованных в формате DMTF. Корпорация Майкрософт могла внести изменения в Исправление незначительных ошибок, соответствовать стандартам документации пакета Microsoft SDK или предоставить дополнительные сведения.

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows Vista<br/>                                                                |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                          |
| Пространство имен<br/>                | Корневой \\ CIMV2<br/>                                                                  |
| MOF<br/>                      | <dl> <dt>CIMWin32. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>CIMWin32.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_КЛУСТЕРИНГСЕРВИЦЕ CIM**](evictnode-method-in-class-cim-clusteringservice.md)
</dt> <dt>

[**\_КЛУСТЕРИНГСЕРВИЦЕ CIM**](cim-clusteringservice.md)
</dt> </dl>

 

