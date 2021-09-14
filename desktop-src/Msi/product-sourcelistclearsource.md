---
description: Метод Саурцелистклеарсаурце удаляет сеть или источник URL-адреса. Принимает тип, исходный путь и источник, в качестве параметров для удаления. Этот метод вызывает Мсисаурцелистклеарсаурце.
ms.assetid: a55676d4-795d-4ffe-8621-ef47c16a936c
title: Метод Product. Саурцелистклеарсаурце
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Product.SourceListClearSource
api_type:
- COM
api_location:
- Msi.dll
ms.openlocfilehash: 4988d0ba9003e087b6aeac58ae5587727067e01c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127057738"
---
# <a name="productsourcelistclearsource-method"></a>Метод Product. Саурцелистклеарсаурце

Метод **саурцелистклеарсаурце** удаляет сеть или источник URL-адреса. Принимает *тип* *, исходный путь и источник*, в качестве параметров для удаления. Этот метод вызывает [**мсисаурцелистклеарсаурце**](/windows/desktop/api/Msi/nf-msi-msisourcelistclearsourcea).

## <a name="syntax"></a>Синтаксис


```JScript
Product.SourceListClearSource(
  Type,
  SourcePath
)
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Тип* 
</dt> <dd>

Тип удаляемого источника: МСИСАУРЦЕТИПЕ \_ Network или мсисаурцетипе \_ URL.

</dd> <dt>

*SourcePath* 
</dt> <dd>

Путь к удаляемому источнику.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Этот метод не возвращает значение.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Версия<br/> | Windows установщик 5,0 на Windows Server 2012, Windows 8, Windows Server 2008 R2 или Windows 7. Windows установщик 4,0 или установщик Windows 4,5 на Windows Server 2008 или Windows Vista. Windows установщик 3,0 или более поздней версии на Windows Server 2003, Windows XP и Windows 2000<br/> |
| DLL<br/>     | <dl> <dt>Msi.dll</dt> </dl>                                                                                                                                                                                                   |
| IID<br/>     | IID \_ ипродукт определен как 000C10A0-0000-0000-C000-000000000046<br/>                                                                                                                                                                                                          |



## <a name="see-also"></a>См. также:

<dl> <dt>

[**Продукта**](product-object.md)
</dt> <dt>

[**мсисаурцелистклеарсаурце**](/windows/desktop/api/Msi/nf-msi-msisourcelistclearsourcea)
</dt> <dt>

[не поддерживается в установщик Windows 2,0 и более ранних версиях](not-supported-in-windows-installer-version-2-0.md)
</dt> </dl>

 

 




