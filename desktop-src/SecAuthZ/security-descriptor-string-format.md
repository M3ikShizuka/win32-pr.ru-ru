---
description: Формат строки дескриптора безопасности — это текстовый формат для хранения или передачи сведений в дескрипторе безопасности.
ms.assetid: 0a226629-084c-40c5-bdd4-ad7355c807cf
title: Формат строки дескриптора безопасности
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 1f338fa3e256f5f0b8dcb27e8260610d8f87594b2e999ab9587389d526165636
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119907354"
---
# <a name="security-descriptor-string-format"></a>Формат строки дескриптора безопасности

**Формат строки дескриптора безопасности** — это текстовый формат для хранения или передачи сведений в дескрипторе безопасности. Функции [**конвертсекуритидескриптортострингсекуритидескриптор**](/windows/desktop/api/Sddl/nf-sddl-convertsecuritydescriptortostringsecuritydescriptora) и [**конвертстрингсекуритидескриптортосекуритидескриптор**](/windows/desktop/api/Sddl/nf-sddl-convertstringsecuritydescriptortosecuritydescriptora) используют этот формат.

Формат является строкой, завершающейся **нулем**, с токенами для указания каждого из четырех основных компонентов дескриптора безопасности: владелец (O:), основная группа (G:), DACL (D:) и SACL (S:).

> [!Note]  
> [*Записи контроля доступа*](/windows/desktop/SecGloss/a-gly) (ACE) и условные элементы ACE имеют разные форматы. Сведения об элементах ACE см. в разделе [строки ACE](ace-strings.md). Сведения об условных ACE см. в разделе [язык определения дескрипторов безопасности для условных элементов ACE](security-descriptor-definition-language-for-conditional-aces-.md).

 


```C++
O:owner_sid
G:group_sid
D:dacl_flags(string_ace1)(string_ace2)... (string_acen)
S:sacl_flags(string_ace1)(string_ace2)... (string_acen)
```



<dl> <dt>

<span id="owner_sid"></span><span id="OWNER_SID"></span>\_идентификатор безопасности владельца
</dt> <dd>

[Строка идентификатора безопасности](sid-strings.md) , определяющая владельца объекта.

</dd> <dt>

<span id="group_sid"></span><span id="GROUP_SID"></span>\_идентификатор безопасности группы
</dt> <dd>

Строка идентификатора безопасности, определяющая основную группу объекта.

</dd> <dt>

<span id="dacl_flags"></span><span id="DACL_FLAGS"></span>\_Флаги DACL
</dt> <dd>

Флаги управления дескрипторами безопасности, применяемые к DACL. Описание этих флагов управления см. в описании функции [**сетсекуритидескрипторконтрол**](/windows/win32/api/securitybaseapi/nf-securitybaseapi-setsecuritydescriptorcontrol) . \_Строка флагов DACL может представлять собой объединение, равное нулю или нескольким следующим строкам.



| Элемент               | Константа в SDDL. h       | Значение                                       |
|-----------------------|--------------------------|-----------------------------------------------|
| Ш                   | \_ЗАЩИЩЕН SDDL          | \_ \_ установлен флаг защищенного списка DACL SE.          |
| AR                  | запрос на \_ Автоматическое \_ НАСЛЕДОВАНие SDDL \_ | \_ \_ \_ установлен флаг автоматического наследования заявки на DACL для SE \_ . |
| AI                  | \_Автоматический \_ НАСЛЕДОВАНный SDDL    | \_ \_ \_ установлен флаг автоматического наследования списка DACL SE.    |
| "без \_ \_ контроля доступа" | \_список ACL со значением NULL SDDL \_          | Список ACL имеет значение null. **Windows server 2008, Windows Vista и Windows server 2003:** Недоступно. |



 

</dd> <dt>

<span id="sacl_flags"></span><span id="SACL_FLAGS"></span>\_Флаги SACL
</dt> <dd>

Флаги управления дескрипторами безопасности, применяемые к SACL. \_Строка флагов SACL использует те же контрольные строки, что и \_ строка флагов DACL.

</dd> <dt>

<span id="string_ace"></span><span id="STRING_ACE"></span>строковый \_ ACE
</dt> <dd>

Строка, описывающая запись ACE в списке DACL или SACL дескриптора безопасности. Описание формата строки ACE см. в разделе [строки ACE](ace-strings.md). Каждая строка ACE заключается в круглые скобки (()).

</dd> </dl>

Ненужные компоненты можно опустить в строке дескриптора безопасности. например, если \_ флаг присутствия SE DACL \_ не задан во входном дескрипторе безопасности, [**конвертсекуритидескриптортострингсекуритидескриптор**](/windows/desktop/api/Sddl/nf-sddl-convertsecuritydescriptortostringsecuritydescriptora) не включает компонент D: в выходную строку. Также можно использовать битовые флаги [**\_ сведений о безопасности**](security-information.md) , чтобы указать компоненты, включаемые в строку дескриптора безопасности.

Формат строки дескриптора безопасности не поддерживает списки ACL **со значением NULL** .

Для обозначения пустого списка ACL строка дескриптора безопасности включает маркер D: или S: без дополнительных строковых данных.

В строке дескриптора безопасности [**Контрольные**](security-descriptor-control.md) биты сохраняются различными способами. SE \_ список DACL \_ присутствует или SE список \_ SACL указывает на \_ наличие токена D: или S: в строке. Другие биты, применимые к спискам DACL или SACL, хранятся в флагах DACL \_ и списках SACL \_ . SE \_ владелец \_ по умолчанию, SE \_ группы по умолчанию \_ , SE \_ DACL \_ по умолчанию, а также заданные по умолчанию биты SE \_ SACL \_ не хранятся в строке дескриптора безопасности. SE \_ сам \_ относительный бит не хранится в строке, но [**конвертстрингсекуритидескриптортосекуритидескриптор**](/windows/desktop/api/Sddl/nf-sddl-convertstringsecuritydescriptortosecuritydescriptora) всегда задает этот бит в выходном дескрипторе безопасности.

В следующих примерах показаны строки дескриптора безопасности и сведения в связанных с ними описательах безопасности.

Строка 1:


```C++
"O:AOG:DAD:(A;;RPWPCCDCLCSWRCWDWOGA;;;S-1-0-0)"
```



Дескриптор безопасности 1:


```C++
    Revision:  0x00000001
    Control:   0x0004
        SE_DACL_PRESENT
    Owner: (S-1-5-32-548)
    PrimaryGroup: (S-1-5-21-397955417-626881126-188441444-512)
DACL
    Revision: 0x02
    Size:     0x001c
    AceCount: 0x0001
    Ace[00]
        AceType:       0x00 (ACCESS_ALLOWED_ACE_TYPE)
        AceSize:       0x0014
        InheritFlags:  0x00
        Access Mask:   0x100e003f
                            READ_CONTROL
                            WRITE_DAC
                            WRITE_OWNER
                            GENERIC_ALL
                            Others(0x0000003f)
        Ace Sid      : (S-1-0-0)
SACL
    Not present
```



Строка 2:


```C++
"O:DAG:DAD:(A;;RPWPCCDCLCRCWOWDSDSW;;;SY)
(A;;RPWPCCDCLCRCWOWDSDSW;;;DA)
(OA;;CCDC;bf967aba-0de6-11d0-a285-00aa003049e2;;AO)
(OA;;CCDC;bf967a9c-0de6-11d0-a285-00aa003049e2;;AO)
(OA;;CCDC;6da8a4ff-0e52-11d0-a286-00aa003049e2;;AO)
(OA;;CCDC;bf967aa8-0de6-11d0-a285-00aa003049e2;;PO)
(A;;RPLCRC;;;AU)S:(AU;SAFA;WDWOSDWPCCDCSW;;;WD)"
```



Дескриптор безопасности 2:


```C++
    Revision:  0x00000001
    Control:   0x0014
        SE_DACL_PRESENT
        SE_SACL_PRESENT
    Owner: (S-1-5-21-397955417-626881126-188441444-512)
    PrimaryGroup: (S-1-5-21-397955417-626881126-188441444-512)
DACL
    Revision: 0x04
    Size:     0x0104
    AceCount: 0x0007
    Ace[00]
        AceType:       0x00 (ACCESS_ALLOWED_ACE_TYPE)
        AceSize:       0x0014
        InheritFlags:  0x00
        Access Mask:   0x000f003f
                            DELETE
                            READ_CONTROL
                            WRITE_DAC
                            WRITE_OWNER
                            Others(0x0000003f)
        Ace Sid:       (S-1-5-18)
    Ace[01]
        AceType:       0x00 (ACCESS_ALLOWED_ACE_TYPE)
        AceSize:       0x0024
        InheritFlags:  0x00
        Access Mask:   0x000f003f
                            DELETE
                            READ_CONTROL
                            WRITE_DAC
                            WRITE_OWNER
                            Others(0x0000003f)
        Ace Sid:       (S-1-5-21-397955417-626881126-188441444-512)
    Ace[02]
        AceType:       0x05 (ACCESS_ALLOWED_OBJECT_ACE_TYPE)
        AceSize:       0x002c
        InheritFlags:  0x00
        Access Mask:   0x00000003
                            Others(0x00000003)
        Flags:         0x00000001, ACE_OBJECT_TYPE_PRESENT
        ObjectType:    GUID_C_USER
        InhObjectType: GUID ptr is NULL
        Ace Sid:       (S-1-5-32-548)
    Ace[03]
        AceType:       0x05 (ACCESS_ALLOWED_OBJECT_ACE_TYPE)
        AceSize:       0x002c
        InheritFlags:  0x00
        Access Mask:   0x00000003
                            Others(0x00000003)
        Flags:         0x00000001, ACE_OBJECT_TYPE_PRESENT
        ObjectType:    GUID_C_GROUP
        InhObjectType: GUID ptr is NULL
        Ace Sid:       (S-1-5-32-548)
    Ace[04]
        AceType:       0x05 (ACCESS_ALLOWED_OBJECT_ACE_TYPE)
        AceSize:       0x002c
        InheritFlags:  0x00
        Access Mask:   0x00000003
                            Others(0x00000003)
        Flags:         0x00000001, ACE_OBJECT_TYPE_PRESENT
        ObjectType:    GUID_C_LOCALGROUP
        InhObjectType: GUID ptr is NULL
        Ace Sid:       (S-1-5-32-548)
    Ace[05]
        AceType:       0x05 (ACCESS_ALLOWED_OBJECT_ACE_TYPE)
        AceSize:       0x002c
        InheritFlags:  0x00
        Access Mask:   0x00000003
                            Others(0x00000003)
        Flags:         0x00000001, ACE_OBJECT_TYPE_PRESENT
        ObjectType:    GUID_C_PRINT_QUEUE
        InhObjectType: GUID ptr is NULL
        Ace Sid:       (S-1-5-32-550)
    Ace[06]
        AceType:       0x00 (ACCESS_ALLOWED_ACE_TYPE)
        AceSize:       0x0014
        InheritFlags:  0x00
        Access Mask:   0x00020014
                            READ_CONTROL
                            Others(0x00000014)
        Ace Sid:       (S-1-5-11)
    SACL
        Revision: 0x02
        Size:     0x001c
        AceCount: 0x0001
        Ace[00]
            AceType:       0x02 (SYSTEM_AUDIT_ACE_TYPE)
            AceSize:       0x0014
            InheritFlags:  0xc0
                SUCCESSFUL_ACCESS_ACE_FLAG
                FAILED_ACCESS_ACE_FLAG
            Access Mask:    0x000d002b
                                DELETE
                                WRITE_DAC
                                WRITE_OWNER
                                Others(0x0000002b)
            Ace Sid:       (S-1-1-0)
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Строки ACE](ace-strings.md)
</dt> <dt>

[Язык определения дескрипторов безопасности для условных элементов ACE](security-descriptor-definition-language-for-conditional-aces-.md)
</dt> </dl>

 

 
