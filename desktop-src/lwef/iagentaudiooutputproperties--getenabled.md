---
title: Иажентаудиуутпутпропертиес
description: Иажентаудиуутпутпропертиес
ms.assetid: a1e555e1-98f1-4a3d-b6ba-4cd35348db2b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1a8f5247a767f82a66920f4c27b48d33044336d5b6d179b68587b06c95c2b502
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "120062044"
---
# <a name="iagentaudiooutputpropertiesgetenabled"></a>Иажентаудиуутпутпропертиес:: enable

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

``` syntax
HRESULT GetEnabled(
long * pbEnabled  // address of variable for audio output Enabled setting 
);                      
```

Получает значение, указывающее, включен ли речевой вывод символов.

-   Возвращает значение S \_ , чтобы указать, что операция выполнена успешно.

<dl> <dt>

<span id="pbEnabled"></span><span id="pbenabled"></span><span id="PBENABLED"></span>*пбенаблед*
</dt> <dd>

Адрес переменной, принимающей **значение true** , если речевой вывод включен и **значение false** в случае отключения.

</dd> </dl>

Поскольку этот параметр влияет на речевой вывод (TTS и звуковой файл) для всех символов, только пользователь может изменить это свойство на странице свойств Microsoft Agent.

 

 




