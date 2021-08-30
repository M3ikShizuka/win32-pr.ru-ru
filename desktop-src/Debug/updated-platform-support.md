---
description: При необходимости библиотека DbgHelp была расширена для поддержки как 32, так и 64-разрядных Windows.
ms.assetid: 34ec8cd3-3260-441d-b55f-4ea21c736eb1
title: Поддержка платформы обновлена
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 44389b0b46782318b3f017fe1baf8c2c0580d6993f9de4dfaa9ece64feae8c17
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119912377"
---
# <a name="updated-platform-support"></a>Поддержка платформы обновлена

При необходимости библиотека DbgHelp была расширена для поддержки как 32, так и 64-разрядных Windows. Исходные функции и определения структур по-прежнему находятся в DbgHelp. h, но существуют также обновленные версии этих определений, совместимые с 64-разрядными Windows. Если в коде используются обновленные функции, их можно скомпилировать как для 32, так и для 64-разрядной Windows. Код также будет более эффективным, так как исходные функции просто вызывают обновленные функции для выполнения работы.

Например, DbgHelp. h содержит определения для **симунлоадмодуле** (исходная функция) и **SymUnloadModule64** (Обновленная функция). Эти определения практически идентичны, но используют разные типы для параметра *басеофдлл* . (**Симунлоадмодуле** использует тип **DWORD** , а **SymUnloadModule64** использует тип **DWORD64** .) При написании кода для использования **SymUnloadModule64** его можно скомпилировать как для 32, так и для 64-разрядного Windows. Код также более эффективен, чем если бы он вызывал **симунлоадмодуле**.

Ниже приведен список обновленных функций.

<dl>

[**EnumerateLoadedModules64**](/windows/desktop/api/Dbghelp/nf-dbghelp-enumerateloadedmodules)  
[**StackWalk64**](/windows/desktop/api/DbgHelp/nf-dbghelp-stackwalk)  
[**SymEnumerateModules64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symenumeratemodules)  
[**SymEnumerateSymbols64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symenumeratesymbols)  
[**SymFunctionTableAccess64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symfunctiontableaccess)  
[**SymGetLineFromAddr64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetlinefromaddr)  
[**SymGetLineFromName64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetlinefromname)  
[**SymGetLineNext64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetlinenext)  
[**SymGetLinePrev64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetlineprev)  
[**SymGetModuleBase64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetmodulebase)  
[**SymGetModuleInfo64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetmoduleinfo)  
[**SymGetSymFromAddr64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetsymfromaddr)  
[**SymGetSymFromName64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetsymfromname)  
[**SymGetSymNext64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetsymnext)  
[**SymGetSymPrev64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symgetsymprev)  
[**SymLoadModule64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symloadmodule)  
[**SymRegisterCallback64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symregistercallback)  
[**SymRegisterFunctionEntryCallback64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symregisterfunctionentrycallback)  
[**SymUnDName64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symundname)  
[**SymUnloadModule64**](/windows/desktop/api/Dbghelp/nf-dbghelp-symunloadmodule)  
</dl>

Ниже приведен список обновленных структур.

<dl>

[**ADDRESS64**](/windows/desktop/api/DbgHelp/ns-dbghelp-address)  
[**IMAGEHLP \_ отложенный \_ символ \_ LOAD64**](/windows/desktop/api/DbgHelp/ns-dbghelp-imagehlp_deferred_symbol_load)  
[**IMAGEHLP \_ дубликат \_ SYMBOL64**](/windows/desktop/api/DbgHelp/ns-dbghelp-imagehlp_duplicate_symbol)  
[**IMAGEHLP \_ LINE64**](/windows/desktop/api/DbgHelp/ns-dbghelp-imagehlp_line)  
[**IMAGEHLP \_ MODULE64**](/windows/desktop/api/DbgHelp/ns-dbghelp-imagehlp_module)  
[**IMAGEHLP \_ SYMBOL64**](/windows/desktop/api/DbgHelp/ns-dbghelp-imagehlp_symbol)  
[**KDHELP64**](/windows/desktop/api/DbgHelp/ns-dbghelp-kdhelp)  
[**STACKFRAME64**](/windows/desktop/api/DbgHelp/ns-dbghelp-stackframe)  
</dl>

 

 



