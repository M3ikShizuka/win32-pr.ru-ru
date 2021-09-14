---
title: Захват размера (Справочник по элементам пользовательского интерфейса MSAA)
description: Захват размера — это Специальный указатель мыши в правом нижнем углу окна, который позволяет пользователю щелкнуть и перетащить захват размера, чтобы изменить размер окна.
ms.assetid: 886b27b3-e88d-47a1-85f3-a55bd14c7a7c
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 9fb7180a8936aff46903257e6be8ca4ab7f0e5b8
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127064082"
---
# <a name="size-grip-msaa-ui-element-reference"></a>Захват размера (Справочник по элементам пользовательского интерфейса MSAA)

Захват размера — это Специальный указатель мыши в правом нижнем углу окна, который позволяет пользователю щелкнуть и перетащить захват размера, чтобы изменить размер окна.

## <a name="iaccessible-methods"></a>Методы IAccessible

Захват размера поддерживает следующие методы [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :

-   [**акчиттест**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acchittest)
-   [**акклокатион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-acclocation)
-   [**аккнавигате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-accnavigate)

## <a name="iaccessible-properties"></a>Свойства IAccessible

Захват размера поддерживает следующие свойства [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) :



| Свойство.                                                                   | Комментарии                                                                                                                                                               |
|----------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**получить \_ аккдескриптион**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accdescription) | Свойство **Description** — может использоваться для изменения ширины и высоты окна.                                                                                   |
| [**получить \_ аккнаме**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accname)               | Свойство **Name** имеет значение "поле size".                                                                                                                                   |
| [**получить \_ аккпарент**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accparent)           | Окно, содержащее захват размера.                                                                                                                                |
| [**получить \_ аккроле**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accrole)               | Свойство **Role** — [**\_ \_ захват системы роли**](object-roles.md).                                                                                  |
| [**получить \_ аккстате**](/windows/desktop/api/Oleacc/nf-oleacc-iaccessible-get_accstate)             | Значение свойства **State** равно нулю, что означает, что объект является видимым, или [**Система состояний \_ \_ невидима**](object-state-constants.md). |



 

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[IAccessible](/windows/desktop/api/oleacc/nn-oleacc-iaccessible)
</dt> </dl>

 

 




