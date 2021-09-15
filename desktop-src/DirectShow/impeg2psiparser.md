---
description: реализация этого интерфейса предоставляется в виде образца кода с помощью пакета SDK для DirectShow.
ms.assetid: a18fc6b6-f37e-4c87-9150-0504333d33c2
title: Интерфейс IMpeg2PsiParser
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IMpeg2PsiParser
api_type:
- COM
api_location: ''
ms.openlocfilehash: 51f0f3373c67da75c50ecc2f6bc234e0351f5dc3
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461939"
---
# <a name="impeg2psiparser-interface"></a>Интерфейс IMpeg2PsiParser

реализация этого интерфейса предоставляется в виде образца кода с помощью пакета SDK для DirectShow. он не является поддерживаемым DirectShow API.

`IMpeg2PsiParser`интерфейс извлекает сведения о программе (PSI) из фильтра средства синтаксического анализа PSI, который предоставляется в DirectShow SDK в качестве образца фильтра. Приложение может использовать этот фильтр для отображения идентификаторов программ (PID) в фильтре демультиплексора MPEG-2.

## <a name="members"></a>Элементы

Интерфейс **IMpeg2PsiParser** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **IMpeg2PsiParser** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **IMpeg2PsiParser** содержит следующие методы.



| Метод                                                                             | Описание                                                                               |
|:-----------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------|
| [**финдрекордпрограммаппид**](/previous-versions/windows/desktop/legacy/dd407137(v=vs.85))         | Находит идентификатор таблицы схемы программы (ПЛТ) для программы с учетом номера программы.<br/> |
| [**жеткаунтофелементаристреамс**](impeg2psiparser-getcountofelementarystreams.md) | Возвращает количество простейших потоков в указанной программе.<br/>             |
| [**жеткаунтофпрограмс**](impeg2psiparser-getcountofprograms.md)                   | Возвращает количество программ в транспортном потоке.<br/>                      |
| [**жетпатверсионнумбер**](impeg2psiparser-getpatversionnumber.md)                 | Извлекает \_ поле номера версии из таблицы взаимосвязей программ (PAT).<br/>  |
| [**жетпмтверсионнумбер**](impeg2psiparser-getpmtversionnumber.md)                 | Извлекает \_ поле номера версии из указанного типа ПЛТ.<br/>                      |
| [**жетрекорделементарипид**](/previous-versions/windows/desktop/legacy/dd376623(v=vs.85))           | Получает назначение PID для указанного простейшего потока в программе.<br/>   |
| [**жетрекордпрограммаппид**](/previous-versions/windows/desktop/legacy/dd376624(v=vs.85))           | Получает назначение PID для указанного типа ПЛТ.<br/>                              |
| [**жетрекордпрограмнумбер**](impeg2psiparser-getrecordprogramnumber.md)           | Возвращает номер программы для указанной программы.<br/>                          |
| [**жетрекордстреамтипе**](/previous-versions/windows/desktop/legacy/dd376626(v=vs.85))                 | Извлекает тип потока для указанного простейшего потока в программе.<br/>      |
| [**жеттранспортстреамид**](impeg2psiparser-gettransportstreamid.md)               | Получает поле идентификатора транспортного \_ потока \_ из Pat.<br/>                        |



 

## <a name="see-also"></a>См. также раздел

<dl> <dt>

[Образец фильтра средства синтаксического анализа PSI](psi-parser-filter-sample.md)
</dt> </dl>

 

 
