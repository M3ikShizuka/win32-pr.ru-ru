---
title: Регистрация компонентов
description: Регистрация компонентов
ms.assetid: d7fd231b-17ec-42ad-9144-df7ed5ffb17b
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5d683ae419466d62d764283cfa8706981de402a9
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369693"
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

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[Регистрация приложений COM](registering-com-applications.md)
</dt> </dl>

 

 