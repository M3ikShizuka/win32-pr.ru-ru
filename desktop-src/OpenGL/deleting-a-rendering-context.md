---
title: Удаление контекста подготовки к просмотру
description: В следующем примере кода показано, как удалить контекст визуализации OpenGL при закрытии окна OpenGL. Это продолжение сценария, используемого при создании контекста отрисовки и его актуальности.
ms.assetid: 562c4698-f5bb-418a-8479-0df07e9834e5
keywords:
- OpenGL на Windows, контексты отрисовки
- Контексты отрисовки OpenGL
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 621abd0de46c874f40568f8361191b25df329f0f
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127260280"
---
# <a name="deleting-a-rendering-context"></a>Удаление контекста подготовки к просмотру

В следующем примере кода показано, как удалить контекст визуализации OpenGL при закрытии окна OpenGL. Это продолжение сценария, используемого при [создании контекста отрисовки и его актуальности](creating-a-rendering-context-and-making-it-current.md).


```C++
// a window is about to be destroyed  
case WM_DESTROY: 
    { 
    // local variables  
    HGLRC    hglrc; 
    HDC      hdc ; 
 
    // if the thread has a current rendering context ...  
    if(hglrc = wglGetCurrentContext()) { 
 
        // obtain its associated device context  
        hdc = wglGetCurrentDC() ; 
 
        // make the rendering context not current  
        wglMakeCurrent(NULL, NULL) ; 
 
        // release the device context  
        ReleaseDC (hwnd, hdc) ; 
 
        // delete the rendering context  
        wglDeleteContext(hglrc); 
 
        }
```



 

 




