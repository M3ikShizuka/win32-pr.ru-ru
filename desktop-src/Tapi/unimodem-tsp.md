---
description: Драйвер Unimodem, или универсальный модем, TSP (Унимдм. TSP) предоставляет доступ практически ко всем стандартным модемам.
ms.assetid: 1ea60477-f6c9-44ae-969c-515dfb0c607e
title: TSP Unimodem
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 115cc4fd159b2e62062171131f583bad19dc9b00
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127168852"
---
# <a name="unimodem-tsp"></a>TSP Unimodem

Драйвер Unimodem, или универсальный модем, TSP (Унимдм. TSP) предоставляет доступ практически ко всем стандартным модемам. Он поддерживает радиомодемы, поддерживающие двустороннюю потоковую передачу. Поддерживаются звуковые MSP и управление потоком. (обратите внимание, что Unimodem в Windows NT 4,0 или более ранней версии не поддерживает голосовые модемы, поэтому прямое управление потоком невозможно).

Этот TSP поддерживает значение [**типа адреса**](./lineaddresstype--constants.md) линеаддресстипе \_ PHONENUMBER. Если программист хочет использовать правила набора номера, интерфейс TAPI 3 [**итаддресстранслатион**](/windows/win32/api/tapi3if/nn-tapi3if-itaddresstranslation) или функция [**линетранслатеаддресс**](/windows/win32/api/tapi/nf-tapi-linetranslateaddress) TAPI 2 должны использоваться для получения набора строк из номера телефона в каноническом формате.

TSP Unimodem устанавливается вместе с операционными системами Windows Server 2003, Windows XP, Windows 2000, Windows NT, Windows Millennium Edition, Windows 98 и Windows 95.

 

 
