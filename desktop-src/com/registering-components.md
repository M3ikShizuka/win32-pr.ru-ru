---
title: Регистрация компонентов
description: Регистрация компонентов
ms.assetid: d7fd231b-17ec-42ad-9144-df7ed5ffb17b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: b58a987bba4ef7767cfc7346730f5f22e2c1eaab8ae3eed76cd33be0ad778902
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119992304"
---
# <a name="registering-components"></a>Регистрация компонентов

При установке следующих типов приложений сведения об установке должны быть добавлены в реестр, обычно через программу установки:

-   Серверные приложения
-   Приложения-контейнеры и серверы
-   Приложения контейнеров, разрешающие связывание с внедренными объектами

Для всех трех экземпляров Зарегистрируйте сведения о библиотеке COM (DLL) и сведения о конкретном приложении.

Библиотека DLL регистрирует сведения для всех своих компонентов путем экспорта [**DllRegisterServer**](/windows/win32/api/olectl/nf-olectl-dllregisterserver) и [**DllUnregisterServer**](/windows/win32/api/olectl/nf-olectl-dllunregisterserver). Используйте следующие функции для регистрации и отмены регистрации компонента:

-   [**RegOpenKeyEx**](/windows/desktop/api/winreg/nf-winreg-regopenkeyexa)
-   [**регкреатекэйекс**](/windows/desktop/api/winreg/nf-winreg-regcreatekeyexa)
-   [**RegSetValueEx**](/windows/desktop/api/winreg/nf-winreg-regsetvalueexa)
-   [**реженумкэйекс**](/windows/desktop/api/winreg/nf-winreg-regenumkeyexa)
-   [**регделетекэй**](/windows/desktop/api/winreg/nf-winreg-regdeletekeya)
-   [**Ошибка RegCloseKey**](/windows/desktop/api/winreg/nf-winreg-regclosekey)

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Регистрация приложений COM](registering-com-applications.md)
</dt> </dl>

 

 