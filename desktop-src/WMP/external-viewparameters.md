---
title: External. Виевпараметерс
description: Обратите внимание, что в этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. | External. Виевпараметерс
ms.assetid: 0afabe35-2857-413a-a662-1a76d3fb75fe
keywords:
- External. виевпараметерс проигрыватель Windows Media
topic_type:
- apiref
api_name:
- External.viewParameters
api_location:
- wmp.dll
api_type:
- DllExport
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: ea0adec580a68bd3f6b92beef1de814729848179
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127241792"
---
# <a name="externalviewparameters"></a>External. Виевпараметерс

> [!Note]  
> В этом разделе описываются функции, предназначенные для использования в Интернет-магазинах. Использование этой функции вне контекста Интернет-магазина не поддерживается.

 

свойство **виевпараметерс** извлекает параметры, связанные с текущим представлением, в проигрыватель Windows Media.

## <a name="syntax"></a>Синтаксис

**Window. external. Виевпараметерс**

## <a name="possible-values"></a>Возможные значения

Это свойство возвращает **строку**, доступную только для чтения.

## <a name="remarks"></a>Remarks

Это свойство извлекает параметры, которые ранее были заданы в Интернет-магазине. Например, в Интернет-магазине можно указать параметры представления в параметре *виевпарамс* метода [Чанжевиев](external-changeview.md) или параметр *params* метода [чанжевиевонлинелист](external-changeviewonlinelist.md) .

параметры представления не обрабатываются проигрыватель Windows Media. Они создаются Интернет-магазином и имеют значение только в Интернет-магазине.

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|------------------------------------------------------------------------------------|
| Версия<br/> | проигрыватель Windows Media 11.<br/>                                                |
| DLL<br/>     | <dl> <dt>Wmp.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Внешний объект для Интернет-магазинов типа 1**](external-object-for-type-1-online-stores.md)
</dt> </dl>

 

 





