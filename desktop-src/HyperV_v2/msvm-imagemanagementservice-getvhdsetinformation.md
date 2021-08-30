---
description: Извлекает сведения о файле набора виртуальных жестких дисков.
ms.assetid: efdfd4c6-b762-4369-add3-e152652c6802
title: Метод Жетвхдсетинформатион класса Msvm_ImageManagementService
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Msvm_ImageManagementService.GetVHDSetInformation
api_type:
- COM
api_location:
- vmms.exe
ms.openlocfilehash: 7777ef26c7c68de05e6488e7ffc80e80179e58dcd33793b078299959da17bd75
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120046684"
---
# <a name="getvhdsetinformation-method-of-the-msvm_imagemanagementservice-class"></a>Метод Жетвхдсетинформатион \_ класса) мсвм

Извлекает сведения о файле набора виртуальных жестких дисков.

## <a name="syntax"></a>Синтаксис


```mof
uint32 GetVHDSetInformation(
  [in]  string              VHDSetPath,
  [in]  uint32              AdditionalInformation[],
  [out] string              Information,
  [out] CIM_ConcreteJob REF Job
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Вхдсетпас* \[ окне\]
</dt> <dd>

Полный путь, указывающий расположение файла набора виртуальных жестких дисков.

</dd> <dt>

*Аддитионалинформатион* \[ окне\]
</dt> <dd>

Массив, указывающий, какие дополнительные сведения следует собрать о файле набора виртуальных жестких дисков. Каждая запись в массиве является типом дополнительной информации. Если этот параметр имеет значение NULL, дополнительные сведения не извлекаются.

<dt>

<span id="Unknown"></span><span id="unknown"></span><span id="UNKNOWN"></span>

**Неизвестно** (0)


</dt> <dd></dd> <dt>

<span id="Other"></span><span id="other"></span><span id="OTHER"></span>

**Другое** (1)


</dt> <dd></dd> <dt>

<span id="Paths"></span><span id="paths"></span><span id="PATHS"></span>

**Пути** (2)


</dt> <dd></dd> </dl> </dd> <dt>

*Сведения о* \[ заполняет\]
</dt> <dd>

В случае успеха этот объект содержит сведения для запрошенного файла набора виртуальных жестких дисков. Это встроенный экземпляр [**мсвм \_ вхдсетинформатион**](msvm-vhdsetinformation.md).

</dd> <dt>

*Задание* \[ заполняет\]
</dt> <dd>

Ссылка на задание (может иметь значение null, если задача завершена).

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод возвращает одно из следующих значений:

<dl> <dt>

**Завершено без ошибок** (0)
</dt> <dt>

**Параметры метода проверены — задание запущено** (4096)
</dt> <dt>

**Сбой** (32768)
</dt> <dt>

**Отказано в доступе** (32769)
</dt> <dt>

**Не поддерживается** (32770)
</dt> <dt>

**Состояние неизвестно** (32771)
</dt> <dt>

**Время ожидания** (32772)
</dt> <dt>

**Недопустимый параметр** (32773)
</dt> <dt>

**Система используется** (32774)
</dt> <dt>

**Недопустимое состояние для этой операции** (32775)
</dt> <dt>

**Неверный тип данных** (32776)
</dt> <dt>

**Система недоступна** (32777)
</dt> <dt>

**Недостаточно памяти** (32778)
</dt> <dt>

**Файл не найден** (32779)
</dt> </dl>

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 10 \[ только классические приложения\]<br/>                                                             |
| Минимальная версия сервера<br/> | Windows Server 2016<br/>                                                                          |
| Пространство имен<br/>                | Корневая \\ виртуализация \\ версии 2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>Виндовсвиртуализатион. v2. mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Мсвм \_ )**](msvm-imagemanagementservice.md)
</dt> </dl>

 

 




