---
title: Рисование с помощью двойных буферов
description: Двойные буферы плавно переходят между одним изображением и другим на экране.
ms.assetid: 10801cc7-d26c-4bfd-95c0-f352a1c7a1f5
keywords:
- OpenGL на Windows, двойные буферы
- Двойная буферизация OpenGL
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: bbe52d427467b2a6e460ea56a9e72e580ea6f97d
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461648"
---
# <a name="drawing-with-double-buffers"></a>Рисование с помощью двойных буферов

Двойные буферы плавно переходят между одним изображением и другим на экране. Переключение буферов обычно происходит в конце последовательности команд рисования. по умолчанию реализация OpenGL в Windows выводит в буфер, расположенный вне экрана; После завершения рисования вызовите функцию [**свапбуфферс**](/windows/desktop/api/wingdi/nf-wingdi-swapbuffers) , чтобы скопировать буфер из буфера экрана в буфер экрана. Следующий пример кода готовится к рисованию, вызывает функцию рисования, а затем копирует готовое изображение на экран, если доступна двойная буферизация.


```C++
void myRedraw(void) 
{ 
    // set up for drawing commands  
    glMatrixMode(GL_PROJECTION); 
    glLoadIdentity(); 
    gluPerspective(45, 1.0, 0.1, 100.0); 
 
    // draw our objects  
    myDrawAllObjects(GL_FALSE); 
 
    // if we're double-buffering ...  
    if (bDoubleBuffering)  
 
        // ...draw the copied image to the screen  
        SwapBuffers(hdc); 
}
```



Следующий пример кода получает контекст устройства окна, отображает сцену, копирует изображение на экран (для отображения отрисовки), а затем освобождает контекст устройства.


```C++
hdc = GetDC(hwnd); 
mySceneRenderingFunction(); 
SwapBuffers(hdc); 
ReleaseDC(hWnd, hdc);
```



 

 




