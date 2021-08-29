---
description: Интерфейс Иинсталлатионресулт определяет следующие свойства.
ms.assetid: bd6cd5ae-2e43-4ac3-8ce7-ac80b7fc5cb8
title: Свойства Иинсталлатионресулт
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 04760f6e1f7505e883b0b4208c0b4b189afc9bd8e98afa4f2b8b429ff12a33eb
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119611274"
---
# <a name="iinstallationresult-properties"></a>Свойства Иинсталлатионресулт

Интерфейс [**иинсталлатионресулт**](/windows/desktop/api/Wuapi/nn-wuapi-iinstallationresult) определяет следующие свойства.



| Свойство                                                     | Описание                                                                                                                            |
|--------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| [**HResult**](/windows/desktop/api/Wuapi/nf-wuapi-iinstallationresult-get_hresult)               | Возвращает **значение HRESULT** исключения (при его наличии), которое возникает во время установки.                                                 |
| [**RebootRequired**](/windows/desktop/api/Wuapi/nf-wuapi-iinstallationresult-get_rebootrequired) | Возвращает логическое значение, указывающее, требуется ли перезагрузка компьютера для завершения установки или удаления обновления. |
| [**ResultCode**](/windows/desktop/api/Wuapi/nf-wuapi-iinstallationresult-get_resultcode)         | Возвращает значение [**оператионресулткоде**](/windows/win32/api/wuapi/ne-wuapi-operationresultcode) , указывающее результат операции над обновлением.               |



 

 

 



