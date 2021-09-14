---
description: ICEM13 проверяет, что модуль слияния не содержит сборок политики издателя и конфигурации.
ms.assetid: 1281ee21-a154-4275-a9e6-6e92fff548ed
title: ICEM13
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 3286906cf162f24dce7105835544c3a387993ac6
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127067933"
---
# <a name="icem13"></a>ICEM13

ICEM13 проверяет, что модуль слияния не содержит сборок политики издателя и конфигурации. Publisher сборки политики и конфигурации не должны включаться в модули слияния, предназначенные для распространения, так как это может повлиять на другие приложения на компьютере пользователя.

этот ицем доступен в файле мержемод. cub, который входит в состав пакета SDK для установщик Windows 2,0 и более поздних версий. дополнительные сведения см. в разделе [Windows SDK компонентов для разработчиков установщик Windows](platform-sdk-components-for-windows-installer-developers.md).

## <a name="result"></a>Результат

ICEM13 отправляет предупреждающее сообщение, если обнаруживает компонент, указанный в поле Component [таблицы мсиассембли](msiassembly-table.md) модуля слияния, которая является политикой издателя или сборкой конфигурации.

## <a name="example"></a>Пример

ICEM13 отправляет следующее предупреждающее сообщение при обнаружении строки в [таблице мсиассембли](msiassembly-table.md) с компонентом " \[ 1 \] ", указанным в поле Component, которое является политикой издателя или сборкой конфигурации, включенной в модуль слияния.

``` syntax
This entry Component_=`[1]` in MsiAssembly Table is a Policy/Configuration Assembly. A Publisher Policy/Configuration assembly should not be redistributed with a merge module. Policy/Configuration may impact other applications and should only be installed with products.
```

можно установить политику издателя и сборки конфигурации с помощью установщик Windows, поэтому не рекомендуется распространять эти сборки в модулях слияния.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Ссылка на модуль слияния ICE](merge-module-ice-reference.md)
</dt> </dl>

 

 



