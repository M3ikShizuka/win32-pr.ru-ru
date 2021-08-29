---
title: Свойство Хелпконтекстид (объект коллекции Commands)
description: Сведения о свойстве Хелпконтекстид объекта коллекции Commands. не рекомендуется использовать Microsoft Agent на Windows 7.
ms.assetid: 8b8ac1c6-1a34-45f1-a0a6-2ae14ad6adef
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 5b0635f62350d0bea31afda09b04e6489fe7f0ccb33173adb6c2aeb69a814265
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119725704"
---
# <a name="helpcontextid-property-commands-collection-object"></a>Свойство Хелпконтекстид (объект коллекции Commands)

\[Microsoft Agent является устаревшим по отношению к Windows 7 и может быть недоступен в последующих версиях Windows.\]

<dl> <dt>

<span id="Description"></span><span id="description"></span><span id="DESCRIPTION"></span>**Nописание**
</dt> <dd>

Возвращает или задает связанный контекстный номер для объекта [**Commands**](/windows/desktop/lwef/the-commands-collection-object) . Используется для предоставления контекстной справки для объекта **Commands** .

</dd> <dt>

<span id="Syntax"></span><span id="syntax"></span><span id="SYNTAX"></span>**Syntax**
</dt> <dd>

*Символы Agent. ***("**_чарактерид_*_"). Команды ("_*_имя_*_")._ *  \[  =  *Номер* хелпконтекстид\]



| Часть     | Описание                                   |
|----------|-----------------------------------------------|
| *Число* | Целое число, указывающее допустимый контекстный номер. |



 

</dd> </dl>

## <a name="remarks"></a>Remarks

если для приложения был создан файл справки Windows и задано свойство [**HelpFile**](helpfile-property.md) символа, агент автоматически вызывает справку, когда [**хелпмодеон**](helpmodeon-property.md) имеет значение **True** и пользователь выбирает объект [**commands**](/windows/desktop/lwef/the-commands-collection-object) . Если задать номер контекста в **хелпконтекстид**, агент вызывает справку и ищет раздел, определяемый этим номером контекста.

Это свойство применяется только к символу, используемому вашим клиентским приложением. Этот параметр не влияет на другие клиенты символов или других символов клиентского приложения.

> [!Note]  
> для создания файла справки требуется компилятор справки Microsoft Windows.

 

## <a name="see-also"></a>См. также

[**HelpFile, свойство**](helpfile-property.md)


 

 
