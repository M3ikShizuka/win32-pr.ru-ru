---
description: интерфейс иамтимелине предоставляет методы для управления временной шкалой, центральным объектом в службах Microsoft DirectShow editing Services (DES).
ms.assetid: 6750efa0-946c-4ad3-b0df-de55872b94c3
title: Интерфейс Иамтимелине (Кедит. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimeline
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: fc4374a198232625b87448004b667ccd8ce0183b
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892189"
---
# <a name="iamtimeline-interface"></a>Интерфейс Иамтимелине

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`IAMTimeline`интерфейс предоставляет методы для управления временной шкалой, центральным объектом в [службах Microsoft DirectShow editing Services](directshow-editing-services.md) (DES). Временная шкала — это коллекция элементов, упорядоченных по времени, таких как видеоклипы, звуковые клипы, эффекты и переходы между клипами. Модуль подготовки отчетов использует временную шкалу для создания графа фильтра, из которого приложение может формировать отображаемые выходные данные.

`IAMTimeline` выполняет три основные службы. Он

-   Создает объекты на временной шкале.
-   Выступает в качестве контейнера для этих объектов.
-   Задает и получает общие параметры временной шкалы.

Чтобы создать объект временной шкалы, вызовите **CoCreateInstance** с идентификатором класса CLSID \_ амтимелине.

## <a name="members"></a>Элементы

Интерфейс **иамтимелине** наследует от интерфейса [**IUnknown**](/windows/win32/api/unknwn/nn-unknwn-iunknown) . **Иамтимелине** также имеет следующие типы членов:

-   [Методы](#methods)

### <a name="methods"></a>Методы

Интерфейс **иамтимелине** содержит следующие методы.



| Метод                                                             | Описание                                                                                                                       |
|:-------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
| [**AddGroup**](iamtimeline-addgroup.md)                           | Добавляет группу на временную шкалу.<br/>                                                                                          |
| [**клеараллграупс**](iamtimeline-clearallgroups.md)               | Удаляет все группы из временной шкалы, а также все объекты, содержащиеся в этих группах.<br/>                                |
| [**креатимптиноде**](iamtimeline-createemptynode.md)             | Создает новый объект временной шкалы.<br/>                                                                                         |
| [**еффектсенаблед**](iamtimeline-effectsenabled.md)               | Определяет, включены ли эффекты.<br/>                                                                                |
| [**енаблиффектс**](iamtimeline-enableeffects.md)                 | Включает или отключает все эффекты на временной шкале.<br/>                                                                       |
| [**енаблетранситионс**](iamtimeline-enabletransitions.md)         | Включает или отключает все переходы на временной шкале.<br/>                                                                   |
| [**жеткаунтофтипе**](iamtimeline-getcountoftype.md)               | Извлекает количество объектов указанного типа, содержащихся в указанной группе и всех ее дочерних элементах.<br/> |
| [**жетдефаултеффект**](iamtimeline-getdefaulteffect.md)           | Возвращает результат по умолчанию.<br/>                                                                                          |
| [**жетдефаултеффектб**](iamtimeline-getdefaulteffectb.md)         | Получает результат по умолчанию в виде значения **BSTR** .<br/>                                                                      |
| [**жетдефаултфпс**](iamtimeline-getdefaultfps.md)                 | Возвращает частоту кадров вывода по умолчанию в кадрах в секунду.<br/>                                                         |
| [**жетдефаулттранситион**](iamtimeline-getdefaulttransition.md)   | Извлекает переход по умолчанию.<br/>                                                                                      |
| [**жетдефаулттранситионб**](iamtimeline-getdefaulttransitionb.md) | Извлекает переход по умолчанию в виде значения **BSTR** .<br/>                                                                  |
| [**жетдиртиранже**](iamtimeline-getdirtyrange.md)                 | Не поддерживается.<br/>                                                                                                         |
| [**Длительное время**](iamtimeline-getduration.md)                     | Возвращает длительность временной шкалы.<br/>                                                                                       |
| [**GetDuration2**](iamtimeline-getduration2.md)                   | Получает длительность временной шкалы в виде **Double**.<br/>                                                                       |
| [**Группа**](iamtimeline-getgroup.md)                           | Извлекает указанную группу.<br/>                                                                                           |
| [**жетграупкаунт**](iamtimeline-getgroupcount.md)                 | Извлекает количество групп, содержащихся на временной шкале.<br/>                                                     |
| [**жетинсертмоде**](iamtimeline-getinsertmode.md)                 | Не поддерживается.<br/>                                                                                                         |
| [**IsDirty**](iamtimeline-isdirty.md)                             | Не поддерживается.<br/>                                                                                                         |
| [**ремграупфромлист**](iamtimeline-remgroupfromlist.md)           | Не поддерживается.<br/>                                                                                                         |
| [**сетдефаултеффект**](iamtimeline-setdefaulteffect.md)           | Задает результат по умолчанию.<br/>                                                                                               |
| [**сетдефаултеффектб**](iamtimeline-setdefaulteffectb.md)         | Устанавливает результат по умолчанию как значение **BSTR** .<br/>                                                                           |
| [**сетдефаултфпс**](iamtimeline-setdefaultfps.md)                 | Задает частоту кадров вывода по умолчанию в кадрах в секунду.<br/>                                                              |
| [**сетдефаулттранситион**](iamtimeline-setdefaulttransition.md)   | Задает переход по умолчанию.<br/>                                                                                           |
| [**сетдефаулттранситионб**](iamtimeline-setdefaulttransitionb.md) | Задает переход по умолчанию в качестве значения BSTR.<br/>                                                                           |
| [**сетинсертмоде**](iamtimeline-setinsertmode.md)                 | Не реализован.<br/>                                                                                                       |
| [**сетинтерестранже**](iamtimeline-setinterestrange.md)           | Не реализован.<br/>                                                                                                       |
| [**транситионсенаблед**](iamtimeline-transitionsenabled.md)       | Определяет, включены ли переходы.<br/>                                                                            |
| [**валидатесаурценамес**](iamtimeline-validatesourcenames.md)     | Проверяет имена источников на временной шкале.<br/>                                                                                |



 

## <a name="remarks"></a>Комментарии

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



 

 
