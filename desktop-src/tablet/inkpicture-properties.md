---
description: Этот раздел содержит свойства для элемента управления InkPicture.
ms.assetid: d724c177-af57-4c99-94f2-c70904910b49
title: Свойства InkPicture
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5419d6a72af365af7f663018e121563c263e6b3b
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122476810"
---
# <a name="inkpicture-properties"></a>Свойства InkPicture

Этот раздел содержит свойства для элемента управления InkPicture.




| Свойство | Описание | 
|----------|-------------|
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_autoredraw"><strong>Ауторедрав, свойство</strong></a> | Возвращает или задает значение, указывающее, перерисовывается ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> при недействительности окна (объект <a href="inkdisp-class.md"><strong>инкдисп</strong></a> , который в данный момент связан с элементом управления InkPicture, автоматически перерисовывается, когда окно, связанное с inkpicture, получает сообщение WM_PAINT).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_backcolor"><strong>BackColor</strong></a> | Возвращает или задает цвет фона для элемента управления <a href="inkpicture-control-reference.md">InkPicture</a> . Цвет фона по умолчанию — это цвет фона системного окна, который обычно является белым.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_collectingink"><strong>Коллектингинк, свойство</strong></a> | Возвращает значение, указывающее, собирает ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> рукописный ввод (только время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_collectionmode"><strong>Режиме CollectionMode</strong></a> | Возвращает или задает режим сбора, определяющий, распознаются ли рукописный ввод, жесты или рукописный ввод и жесты при записи пользователем.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_cursors"><strong>Cursor, свойство</strong></a> | Возвращает коллекцию <a href="/windows/desktop/api/msinkaut/nn-msinkaut-iinkcursors"><strong>иинккурсорс</strong></a> , доступную для использования в области рукописного ввода в элементе управления <a href="inkpicture-control-reference.md">InkPicture</a> .<br /> | 
| <a href="/previous-versions/windows/desktop/legacy/ms703274(v=vs.85)"><strong>кустомстрокес</strong></a> | Возвращает коллекцию <a href="/windows/desktop/api/msinkaut/nn-msinkaut-iinkcustomstrokes"><strong>иинккустомстрокес</strong></a> , которая должна быть сохранена с рукописным вводом (только во время разработки).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_defaultdrawingattributes"><strong>DefaultDrawingAttributes, свойство</strong></a> | Возвращает или задает коллекцию <a href="inkdrawingattributes-class.md"><strong>инкдравингаттрибутес</strong></a> по умолчанию, используемую при прорисовке и отображении рукописного ввода (только во время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_desiredpacketdescription"><strong>Десиредпаккетдескриптион, свойство</strong></a> | Возвращает или задает описание пакета для элемента управления <a href="inkpicture-control-reference.md">InkPicture</a> (только время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_dynamicrendering"><strong>Динамикрендеринг, свойство</strong></a> | Возвращает или задает значение, указывающее, будет ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> динамически отображать рукописный ввод при его сборе.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_editingmode"><strong>EditingMode</strong></a> | Возвращает или задает значение, указывающее, находится ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> в режиме рукописного ввода, режиме удаления или режиме правки или выбора.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_enabled"><strong>Включен</strong></a> | Возвращает или задает значение, определяющее, может ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> отвечать на создаваемые пользователем события.<br /><blockquote>[!Note]<br />Это свойство эквивалентно свойству <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_inkenabled"><strong>инкенаблед</strong></a> .</blockquote><br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_erasermode"><strong>ерасермоде</strong></a> | Возвращает или задает значение, указывающее, удаляются ли рукописные данные по штрихам или по точкам.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_eraserwidth"><strong>ерасервидс</strong></a> | Возвращает или задает значение, указывающее ширину кончика пера ластика.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_hwnd"><strong>hWnd</strong></a> | Возвращает описатель окна, к которому привязан элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> . (только время выполнения)<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_ink"><strong>Рукописный ввод</strong></a> | Возвращает или задает объект <a href="inkdisp-class.md"><strong>инкдисп</strong></a> , связанный с элементом управления <a href="inkpicture-control-reference.md">InkPicture</a> (только время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_inkenabled"><strong>инкенаблед</strong></a> | Возвращает или задает значение, указывающее, собирает ли элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> входные данные пера (пакеты в сети Air, курсоры в пределах диапазона и т. д.).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_marginx"><strong>Маргинкс, свойство</strong></a> | Возвращает или задает поле оси x вокруг прямоугольника окна в экранных координатах.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_marginy"><strong>Свойство Margin</strong></a> | Возвращает или задает поле оси y вокруг прямоугольника окна в экранных координатах.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_mouseicon"><strong>Маусеикон, свойство</strong></a> | Возвращает или задает текущий пользовательский значок мыши.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_mousepointer"><strong>MousePointer, свойство</strong></a> | Возвращает или задает значение, указывающее тип указателя мыши, который появляется при наведении указателя мыши на определенную часть элемента управления <a href="inkpicture-control-reference.md">InkPicture</a> .<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_picture"><strong>Снимки</strong></a> | Возвращает графический файл, отображаемый в элементе управления <a href="inkpicture-control-reference.md">InkPicture</a> .<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_renderer"><strong>Свойство модуля подготовки отчетов</strong></a> | Возвращает или задает объект <a href="inkrenderer-class.md"><strong>инкрендерер</strong></a> , используемый для рисования рукописного ввода в элементе управления <a href="inkpicture-control-reference.md">InkPicture</a> (только время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_selection"><strong>Выбор</strong></a> | Возвращает коллекцию <a href="/previous-versions/windows/desktop/legacy/ms703293(v=vs.85)">инкстрокес</a> , выбранную в данный момент в элементе управления <a href="inkpicture-control-reference.md">InkPicture</a> (только время выполнения).<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_sizemode"><strong>SizeMode</strong></a> | Возвращает или задает способ, которым элемент управления обрабатывает размещение и изменение размера изображения.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_supporthighcontrastink"><strong>Суппорсигхконтрастинк, свойство</strong></a> | Возвращает значение, указывающее, отображаются ли рукописные данные только в одном цвете, Color = COLOR_WINDOWTEXT (из вызова Жетсистемметрикс), когда система находится в режиме высокая контрастность.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_supporthighcontrastselectionui"><strong>суппорсигхконтрастселектионуи</strong></a> | Возвращает или задает значение, указывающее, отображаются ли все пользовательские интерфейсы выделения (ограничивающие прямоугольники выделения и маркеры выделения) с высокой контрастностью, когда система находится в режиме высокая контрастность.<br /> | 
| <a href="/windows/desktop/api/msinkaut/nf-msinkaut-iinkpicture-get_tablet"><strong>Свойство планшета</strong></a> | Возвращает объект <a href="/windows/desktop/api/msinkaut/nn-msinkaut-iinktablet"><strong>иинктаблет</strong></a> , который в настоящее время использует элемент управления <a href="inkpicture-control-reference.md">InkPicture</a> для получения входных данных.<br /> | 




 

