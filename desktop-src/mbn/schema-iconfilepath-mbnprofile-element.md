---
description: Содержит путь к файлу значка для соединения.
ms.assetid: 9daf4916-914b-4326-9933-b433cc00b4c1
title: Иконфилепас (Мбнпрофиле), элемент
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ICONFilePath
api_type:
- Schema
ms.openlocfilehash: 6b1e98f76fe2f83ce214076223b5a1439bd0ea45
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127568671"
---
# <a name="iconfilepath-mbnprofile-element"></a>Иконфилепас (Мбнпрофиле), элемент

Элемент **иконфилепас (мбнпрофиле)** содержит путь к файлу значка для соединения.

В пользовательском интерфейсе подключения операционной системы будет отображаться этот значок, когда соединение устанавливается с помощью этого элемента.

При передаче XML для создания профиля в методе [**креатеконнектионпрофиле**](/windows/desktop/api/mbnapi/nf-mbnapi-imbnconnectionprofilemanager-createconnectionprofile) интерфейса [**имбнконнектионпрофилеманажер**](/windows/desktop/api/mbnapi/nn-mbnapi-imbnconnectionprofilemanager) этот путь должен указывать на исходное расположение файла значка. При успешном создании объекта [**имбнконнектионпрофиле**](/windows/desktop/api/mbnapi/nn-mbnapi-imbnconnectionprofile) служба мобильной широкополосной связи скопирует файл значка в внутреннее хранилище, а путь к профилю будет изменен в соответствии с этим.

Файл значка должен иметь формат .bmp с размером 32X32 пикселя.

Этот элемент представляет собой строку длиной до 1024 символов, содержащую абсолютный путь к файлу.

Элемент является необязательным.

``` syntax
<xs:element name="ICONFilePath"
    type="iconFileType"
 />
```

Элемент **иконфилепас** определяется элементом [**мбнпрофиле**](schema-mbnprofile-element.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------|
| Минимальная версия клиента<br/> | \[приложения UWP для классических приложений Windows 7 \|\]<br/> |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                         |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

**Контекст определения элемента в схеме**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> <dt>

**Возможный непосредственный родительский элемент в экземпляре схемы**
</dt> <dt>

[**мбнпрофиле**](schema-mbnprofile-element.md)
</dt> </dl>

 

 




