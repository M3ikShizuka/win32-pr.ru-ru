---
title: Метод Ремовелсфромтслсграуп класса Win32_TSLicenseServer
description: Удаляет сервер лицензий удаленный рабочий стол из группы серверов лицензирования службы удаленных рабочих столов на контроллере домена в том же домене, что и сервер лицензирования.
ms.assetid: 5ed4595b-0668-4dd8-953e-b6fc61088cfd
ms.tgt_platform: multiple
keywords:
- службы удаленных рабочих столов метода Ремовелсфромтслсграуп
- Службы удаленных рабочих столов метода Ремовелсфромтслсграуп, класс Win32_TSLicenseServer
- Класс Win32_TSLicenseServer службы удаленных рабочих столов, метод Ремовелсфромтслсграуп
topic_type:
- apiref
api_name:
- Win32_TSLicenseServer.RemoveLSfromTSLSGroup
api_location:
- TlsWmiProv.dll
api_type:
- COM
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 209e6d57cd7e0a70add3f6d44f6228cc5ab9fdfff3b6443dc3657ff820b1a9d4
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119988524"
---
# <a name="removelsfromtslsgroup-method-of-the-win32_tslicenseserver-class"></a>Метод Ремовелсфромтслсграуп \_ класса Win32 тслиценсесервер

Удаляет сервер лицензий удаленный рабочий стол из группы серверов лицензирования службы удаленных рабочих столов на контроллере домена в том же домене, что и сервер лицензирования.

## <a name="syntax"></a>Синтаксис


```mof
uint32 RemoveLSfromTSLSGroup();
```



## <a name="parameters"></a>Параметры

Этот метод не имеет параметров.

## <a name="return-value"></a>Возвращаемое значение

Если метод завершается с ошибкой, он возвращает ноль. Если метод завершился неудачно, он возвращает ненулевое значение. Список кодов ошибок см. в разделе [службы удаленных рабочих столов коды ошибок поставщика WMI](terminal-services-wmi-provider-error-codes.md).

## <a name="remarks"></a>Remarks

Для вызова этого метода необходимо быть членом группы "Администраторы домена".

файлы MOF-файл (MOF) содержат определения для классов инструментарий управления Windows (WMI) (WMI). файлы MOF не устанавливаются в составе пакета средств разработки программного обеспечения Microsoft Windows Software Development Kit (SDK). Они устанавливаются на сервере при добавлении связанной роли с помощью диспетчер сервера. Дополнительные сведения о файлах MOF см. в разделе [MOF-файл (MOF)](/windows/desktop/WmiSdk/managed-object-format--mof-).

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|-------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Ни одна версия не поддерживается<br/>                                                                 |
| Минимальная версия сервера<br/> | Windows Server 2008<br/>                                                            |
| Пространство имен<br/>                | Root\\CIMv2<br/>                                                                    |
| MOF<br/>                      | <dl> <dt>Тлсвмипров. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>TlsWmiProv.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**\_Тслиценсесервер Win32**](win32-tslicenseserver.md)
</dt> </dl>

 

