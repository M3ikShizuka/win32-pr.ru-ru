---
description: Описывает ошибки поставщика WMI SNMP с 231 по 240.
ms.assetid: edb3dabb-6a65-4285-97d3-f7025d3bb5da
ms.tgt_platform: multiple
title: Ошибки с 231 по 240
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: c5bf38ca62f543122ee937d7759ebd5655470a54
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122880879"
---
# <a name="errors-231-through-240"></a>Ошибки с 231 по 240

Описывает ошибки поставщика WMI SNMP с 231 по 240.

[Неустранимая ошибка 232](#fatal-error-232)

[Неустранимая ошибка 233](#fatal-error-233)

[Неустранимая ошибка 234](#fatal-error-234)

[Неустранимая ошибка 236](#fatal-error-236)

## <a name="fatal-error-232"></a>Неустранимая ошибка 232

<dl> <dt>

<span id="_232__Fatal____fileName___line___Invocation_of_SNMPv1_SMI_OBJECT-TYPE_disallowed_"></span><span id="_232__fatal____filename___line___invocation_of_snmpv1_smi_object-type_disallowed_"></span><span id="_232__FATAL____FILENAME___LINE___INVOCATION_OF_SNMPV1_SMI_OBJECT-TYPE_DISALLOWED_"></span>**<232, Неустранимая>: " &lt; имя_файла &gt; : <Line \#>: вызов НЕРАЗРЕШЕННОГО типа объекта SMI ()**
</dt> <dd>

Ошибка синтаксиса модуля. В MIB использовался вызов **типа объекта** , относящегося к стандарту, но был указан параметр **/v2c** , для которого требуется строгое соответствие синтаксису SNMPv2c.

</dd> </dl>

## <a name="fatal-error-233"></a>Неустранимая ошибка 233

<dl> <dt>

<span id="_233__Fatal_____fileName___line____Invocation_of_SNMPv1_SMI_TRAP-TYPE_disallowed_"></span><span id="_233__fatal_____filename___line____invocation_of_snmpv1_smi_trap-type_disallowed_"></span><span id="_233__FATAL_____FILENAME___LINE____INVOCATION_OF_SNMPV1_SMI_TRAP-TYPE_DISALLOWED_"></span>**<233, Неустранимая>: " &lt; имя_файла &gt; : <Line \#>: вызов из-за НЕРАЗРЕШЕННОГО типа ловушек SMI"**
</dt> <dd>

Ошибка синтаксиса модуля. В MIB использовался вызов **типа ловушки** , заданный в стандарте, но был указан параметр **/v2c** , для которого требуется строгое соответствие синтаксису SNMPv2c.

</dd> </dl>

## <a name="fatal-error-234"></a>Неустранимая ошибка 234

<dl> <dt>

<span id="_234__Fatal____fileName___line____MODULE-IDENTITY_invocation_is_allowed_only_immediately_after_the_IMPORTS_section_"></span><span id="_234__fatal____filename___line____module-identity_invocation_is_allowed_only_immediately_after_the_imports_section_"></span><span id="_234__FATAL____FILENAME___LINE____MODULE-IDENTITY_INVOCATION_IS_ALLOWED_ONLY_IMMEDIATELY_AFTER_THE_IMPORTS_SECTION_"></span>**<234, Неустранимая>: " &lt; имя_файла &gt; : <Line \#>: вызов удостоверения модуля разрешен только сразу после раздела Imports"**
</dt> <dd>

Ошибка синтаксиса модуля. Недопустимый вызов **удостоверения модуля** .

</dd> </dl>

## <a name="fatal-error-236"></a>Неустранимая ошибка 236

<dl> <dt>

<span id="_236__Fatal_____fileName___line____Number_does_not_fit_into_the_32_bit_representation_used_by_the_compiler_"></span><span id="_236__fatal_____filename___line____number_does_not_fit_into_the_32_bit_representation_used_by_the_compiler_"></span><span id="_236__FATAL_____FILENAME___LINE____NUMBER_DOES_NOT_FIT_INTO_THE_32_BIT_REPRESENTATION_USED_BY_THE_COMPILER_"></span>**<236, Неустранимая>: " &lt; имя_файла &gt; : <строка \#>: число не соответствует 32 разрядному представлению, используемому компилятором"**
</dt> <dd>

Ошибка синтаксиса модуля в назначении значения. Имеется ошибка присваивания значения MIB, при которой целочисленное значение настолько велико, что оно должно представлять более 32 бит.

</dd> </dl>

 

 



