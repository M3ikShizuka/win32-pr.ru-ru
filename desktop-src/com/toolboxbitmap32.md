---
title: ToolBoxBitmap32
description: Определяет имя модуля и идентификатор ресурса для точечного рисунка размером 16 x 16, который будет использоваться для кнопки панели инструментов или панели элементов.
ms.assetid: 87b3d8e1-4d54-465c-9e5e-5e4f7391f313
keywords:
- COM раздела реестра ToolBoxBitmap32
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d2ca6208586e961c0b6f8fa666c5731bab38faa6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127253093"
---
# <a name="toolboxbitmap32"></a>ToolBoxBitmap32

Определяет имя модуля и идентификатор ресурса для точечного рисунка размером 16 x 16, который будет использоваться для кнопки панели инструментов или панели элементов.

## <a name="registry-entry"></a>Запись реестра

```
HKEY_LOCAL_MACHINE\SOFTWARE\Classes\CLSID
   {CLSID}
      ToolBoxBitmap32 = filename,  resourceID
```

## <a name="remarks"></a>Комментарии

Это значение **reg \_ SZ** , которое указывает имя модуля и идентификатор ресурса для точечного рисунка.

размер значка стандартного Windows слишком велик для использования в этой цели. Для этого требуются контейнеры элементов управления, имеющие режим конструктора, в котором один выбирает элементы управления и помещает их в разрабатываемую форму.

 

 




