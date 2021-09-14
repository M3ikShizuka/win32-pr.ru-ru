---
title: 'Функции ввода с помощью мыши '
description: 'Функции ввода с помощью мыши '
ms.assetid: a666b25b-a75c-4500-8077-fabe07589a1d
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 08b9dffed2446addaced30341364d2f755fcd4c5
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127242194"
---
# <a name="mouse-input-functions"></a>Функции ввода с помощью мыши 


## <a name="in-this-section"></a>В этом разделе




| Раздел | Описание | 
|-------|-------------|
| <a href="/windows/win32/api/commctrl/nf-commctrl-_trackmouseevent"><strong>_TrackMouseEvent</strong></a><br /> | Отправляет сообщения, когда указатель мыши покидает окно или наводится на окно в течение заданного промежутка времени. Эта функция вызывает <a href="/windows/desktop/api/winuser/nf-winuser-trackmouseevent"><strong>TrackMouseEven</strong></a> , если она существует, в противном случае она эмулирует ее.<br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-dragdetect"><strong>драгдетект</strong></a><br /> | Захватывает мышь и отслеживает ее движение, пока пользователь не отпустит левую кнопку мыши, не нажмет клавишу ESC или не переместит мышь за пределы прямоугольника перетаскивания, в котором находится указанная точка. Ширина и высота прямоугольника перетаскивания задаются <strong>SM_CXDRAG</strong> и <strong>SM_CYDRAG</strong> значениями, возвращаемыми функцией <a href="/windows/desktop/api/winuser/nf-winuser-getsystemmetrics"><strong>жетсистемметрикс</strong></a> .<br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-getcapture"><strong>Захват</strong></a><br /> | Извлекает маркер окна (при его наличии), которое захватило мышь. Захват мыши может осуществляться только по одному окну. Это окно получает ввод с помощью мыши независимо от того, находится ли курсор внутри его границ. <br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-getdoubleclicktime"><strong>жетдаублекликктиме</strong></a><br /> | Извлекает текущее время двойного щелчка мыши. Двойной щелчок — это последовательность из двух щелчков кнопки мыши, вторая в течение заданного времени после первой. Время двойного щелчка — это максимальное число миллисекунд, которое может произойти между первым и вторым щелчком двойного щелчка. Максимальное время двойного щелчка составляет 5000 миллисекунд.<br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-getmousemovepointsex"><strong>жетмаусемовепоинтсекс</strong></a><br /> | Извлекает журнал до 64 предыдущих координат мыши или пера.<br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-mouse_event"><strong>mouse_event</strong></a><br /> | Функция <a href="/windows/desktop/api/winuser/nf-winuser-mouse_event"><strong>mouse_event</strong></a> синтезирования движения мыши и щелчков кнопок.<br /><blockquote>[!Note]<br />Эта функция была заменена. Вместо этого используйте <a href="/windows/desktop/api/winuser/nf-winuser-sendinput"><strong>SendInput</strong></a> .</blockquote><br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-releasecapture"><strong>релеасекаптуре</strong></a><br /> | Освобождает захват мыши из окна в текущем потоке и восстанавливает нормальную обработку ввода мыши. Окно, захваченное мышью, получает все входные данные мыши независимо от положения курсора, за исключением случаев нажатия кнопки мыши, когда активная активная кнопка находится в окне другого потока. <br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-setcapture"><strong>сеткаптуре</strong></a><br /> | Устанавливает захват мыши в указанное окно, принадлежащее текущему потоку.<br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-setdoubleclicktime"><strong>сетдаублекликктиме</strong></a><br /> | Задает время двойного щелчка мыши. Двойной щелчок — это последовательность из двух щелчков кнопки мыши, вторая в течение заданного времени после первой. Время двойного щелчка — это максимальное число миллисекунд, которое может произойти между первым и вторым щелчками двойного щелчка. <br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-swapmousebutton"><strong>свапмаусебуттон</strong></a><br /> | Изменяет значение левой и правой кнопок мыши на противоположное или восстанавливает его. <br /> | 
| <a href="/windows/desktop/api/winuser/nf-winuser-trackmouseevent"><strong>TrackMouseEven</strong></a><br /> | Отправляет сообщения, когда указатель мыши покидает окно или наводится на окно в течение заданного промежутка времени.<br /><blockquote>[!Note]<br />Функция <a href="/windows/win32/api/commctrl/nf-commctrl-_trackmouseevent"><strong>_TrackMouseEvent</strong></a> вызывает <a href="/windows/desktop/api/winuser/nf-winuser-trackmouseevent"><strong>TrackMouseEven</strong></a> , если она существует, в противном случае <strong>_TrackMouseEvent</strong> эмулирует <strong>TrackMouseEven</strong>.</blockquote><br /> | 




 

 

