---
description: Извлекает сведения об указанном процессе.
ms.assetid: c36c023f-7f9a-4ba5-a41f-f2f755a24eb6
title: Функция Звкуеринформатионпроцесс
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- ZwQueryInformationProcess
api_type:
- DllExport
api_location:
- Ntdll.dll
- ntoskrnl.exe
ms.openlocfilehash: af47ecbe69c4c0449cf6e3282e0992e8a513b5a0
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127375005"
---
# <a name="zwqueryinformationprocess-function"></a>Функция Звкуеринформатионпроцесс

\[**Звкуеринформатионпроцесс** может быть изменен или недоступен в будущих версиях Windows. Приложения должны использовать альтернативные функции, перечисленные в этом разделе.\]

Извлекает сведения об указанном процессе.

## <a name="syntax"></a>Синтаксис


```C++
NTSTATUS WINAPI ZwQueryInformationProcess(
  _In_      HANDLE           ProcessHandle,
  _In_      PROCESSINFOCLASS ProcessInformationClass,
  _Out_     PVOID            ProcessInformation,
  _In_      ULONG            ProcessInformationLength,
  _Out_opt_ PULONG           ReturnLength
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Процесшандле* \[ окне\]
</dt> <dd>

Описатель процесса, для которого извлекаются сведения.

</dd> <dt>

*Процессинформатионкласс* \[ окне\]
</dt> <dd>

Тип извлекаемых сведений о процессе. Этот параметр может принимать одно из следующих значений перечисления **процессинфокласс** .




| Значение | Значение | 
|-------|---------|
| <span id="ProcessBasicInformation"></span><span id="processbasicinformation"></span><span id="PROCESSBASICINFORMATION"></span><dl><dt><strong>ПроцессбасиЦинформатион</strong></dt><dt>0</dt></dl> | Получает указатель на структуру ПЕБ, которую можно использовать, чтобы определить, выполняется ли отладка указанного процесса, и уникальное значение, используемое системой для определения указанного процесса. <br /> Для получения этих сведений лучше использовать функции <a href="/windows/desktop/api/debugapi/nf-debugapi-checkremotedebuggerpresent"><strong>чеккремотедебугжерпресент</strong></a> и <a href="/windows/desktop/api/processthreadsapi/nf-processthreadsapi-getprocessid"><strong>GetProcessId</strong></a> .<br /> | 
| <span id="ProcessDebugPort"></span><span id="processdebugport"></span><span id="PROCESSDEBUGPORT"></span><dl><dt><strong>Процессдебугпорт</strong></dt><dt>7</dt></dl> | Извлекает <strong>DWORD_PTR</strong> значение, которое является номером порта отладчика для процесса. Ненулевое значение указывает, что процесс выполняется под управлением отладчика Ring 3.<br /> Лучше использовать функцию <a href="/windows/desktop/api/debugapi/nf-debugapi-checkremotedebuggerpresent"><strong>чеккремотедебугжерпресент</strong></a> или <a href="/windows/desktop/api/debugapi/nf-debugapi-isdebuggerpresent"><strong>исдебугжерпресент</strong></a> .<br /> | 
| <span id="ProcessWow64Information"></span><span id="processwow64information"></span><span id="PROCESSWOW64INFORMATION"></span><dl><dt><strong>ProcessWow64Information</strong></dt><dt>26</dt></dl> | Определяет, выполняется ли процесс в среде WOW64 (WOW64 — эмулятор x86, позволяющий приложениям на основе Win32 работать на 64-разрядной Windows).<br /> Для получения этих сведений лучше использовать функцию <a href="/windows/desktop/api/wow64apiset/nf-wow64apiset-iswow64process"><strong>IsWow64Process</strong></a> .<br /> | 
| <span id="ProcessImageFileName"></span><span id="processimagefilename"></span><span id="PROCESSIMAGEFILENAME"></span><dl><dt><strong>Процессимажефиленаме</strong></dt><dt>27</dt></dl> | Извлекает значение <strong>UNICODE_STRING</strong> , содержащее имя файла изображения для процесса.<br /> | 
| <span id="ProcessBreakOnTermination"></span><span id="processbreakontermination"></span><span id="PROCESSBREAKONTERMINATION"></span><dl><dt><strong>Процессбреаконтерминатион</strong></dt><dt>29</dt></dl> | Извлекает значение типа <strong>ulong</strong> , указывающее, считается ли процесс критическим.<br /><blockquote>[!Note]<br />это значение можно использовать начиная с версии Windows XP с пакетом обновления 3 (SP3). начиная с Windows 8.1 вместо него следует использовать <a href="/windows/desktop/api/processthreadsapi/nf-processthreadsapi-isprocesscritical"><strong>испроцесскритикал</strong></a> .</blockquote><br /> | 
| <span id="ProcessProtectionInformation"></span><span id="processprotectioninformation"></span><span id="PROCESSPROTECTIONINFORMATION"></span><dl><dt><strong>Процесспротектионинформатион</strong></dt><dt>61</dt></dl> | Извлекает значение БАЙТа, указывающее тип защищенного процесса и подписанного процесса.<br /> | 




 

</dd> <dt>

*Процессинформатион* \[ заполняет\]
</dt> <dd>

Указатель на буфер, предоставленный вызывающим приложением, в который функция записывает запрошенные сведения. Размер записываемой информации зависит от значения параметра *процессинформатионкласс* :

<dl> <dt>

<span id="PROCESS_BASIC_INFORMATION"></span><span id="process_basic_information"></span>\_основные \_ сведения об обработке
</dt> <dd>

Если параметр *процессинформатионкласс* имеет значение **процессбасиЦинформатион**, буфер, на который указывает параметр *процессинформатион* , должен быть достаточно большим, чтобы вместить одну **\_ базовую структуру \_ сведений** , имеющую следующий макет:

``` syntax
typedef struct _PROCESS_BASIC_INFORMATION {
    PVOID Reserved1;
    PPEB PebBaseAddress;
    PVOID Reserved2[2];
    ULONG_PTR UniqueProcessId;
    PVOID Reserved3;
} PROCESS_BASIC_INFORMATION;
```

Элемент **уникуепроцессид** указывает на уникальный идентификатор системы для этого процесса. Для получения этих сведений лучше использовать функцию [**GetProcessId**](/windows/win32/api/processthreadsapi/nf-processthreadsapi-getprocessid) .

Элемент **пеббасеаддресс** указывает на структуру [**пеб**](/windows/desktop/api/Winternl/ns-winternl-peb) .

Другие члены этой структуры зарезервированы для внутреннего использования операционной системой.

</dd> <dt>

<span id="ULONG_PTR"></span><span id="ulong_ptr"></span>ULONG- \_ ptr
</dt> <dd>

Если параметр *процессинформатионкласс* имеет значение **ProcessWow64Information**, буфер, на который указывает параметр *процессинформатион* , должен быть достаточно большим для хранения записи **\_ типа ulong**. Если это значение не равно нулю, процесс выполняется в среде WOW64; в противном случае, если значение равно нулю, процесс не выполняется в среде WOW64.

Лучше использовать функцию [**IsWow64Process**](/windows/win32/api/wow64apiset/nf-wow64apiset-iswow64process) , чтобы определить, выполняется ли процесс в среде WOW64.

</dd> <dt>

<span id="UNICODE_STRING"></span><span id="unicode_string"></span>строка в Юникоде \_
</dt> <dd>

Если параметр *процессинформатионкласс* имеет значение **процессимажефиленаме**, буфер, на который указывает параметр *процессинформатион* , должен быть достаточно большим, чтобы вместить **\_ строковую** структуру в Юникоде, а также саму строку. Строка, хранящаяся в элементе **buffer** , является именем файла изображения.

Если буфер слишком мал, функция завершается с ошибкой \_ \_ несоответствия длины сведений о состоянии \_ и параметру *ретурнленгс* присваивается требуемый размер буфера.

</dd> <dt>

<span id="PS_PROTECTION"></span><span id="ps_protection"></span>PS_PROTECTION
</dt> <dd>

Если параметр *процессинформатионкласс* имеет значение **процесспротектионинформатион**, буфер, на который указывает параметр *процессинформатион* , должен быть достаточно большим, чтобы вместить одну структуру **PS_PROTECTION** со следующим макетом:

``` syntax
typedef struct _PS_PROTECTION {
    union {
        UCHAR Level;
        struct {
            UCHAR Type   : 3;
            UCHAR Audit  : 1;                  // Reserved
            UCHAR Signer : 4;
        };
    };
} PS_PROTECTION, *PPS_PROTECTION;
```

Первые 3 бита содержат тип защищенного процесса:

``` syntax
typedef enum _PS_PROTECTED_TYPE {
    PsProtectedTypeNone = 0,
    PsProtectedTypeProtectedLight = 1,
    PsProtectedTypeProtected = 2
} PS_PROTECTED_TYPE, *PPS_PROTECTED_TYPE;
```

Старшие 4 бита содержат подпись защищенного процесса:

``` syntax
typedef enum _PS_PROTECTED_SIGNER {
    PsProtectedSignerNone = 0,
    PsProtectedSignerAuthenticode,
    PsProtectedSignerCodeGen,
    PsProtectedSignerAntimalware,
    PsProtectedSignerLsa,
    PsProtectedSignerWindows,
    PsProtectedSignerWinTcb,
    PsProtectedSignerWinSystem,
    PsProtectedSignerApp,
    PsProtectedSignerMax
} PS_PROTECTED_SIGNER, *PPS_PROTECTED_SIGNER;
```

</dd> </dl> </dd> <dt>

*Процессинформатионленгс* \[ окне\]
</dt> <dd>

Размер буфера, на который указывает параметр *процессинформатион* в байтах.

</dd> <dt>

*Ретурнленгс* \[ out, необязательно\]
</dt> <dd>

Указатель на переменную, в которой функция возвращает размер запрашиваемой информации. Если функция выполнена успешно, это размер информации, записанной в буфер, на который указывает параметр *процессинформатион* , но если буфер слишком мал, это минимальный размер буфера, необходимого для успешного получения информации.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает сообщение об успешном завершении NTSTATUS или код ошибки.

Формы и коды ошибок NTSTATUS перечислены в файле заголовка NTSTATUS. h, доступном в наборе DDK. они описаны в документации по DDK в разделе Kernel-Mode архитектура драйвера/руководство по проектированию/средства программирования драйверов/регистрация ошибок.

## <a name="remarks"></a>Remarks

функция **звкуеринформатионпроцесс** и возвращаемые ею структуры являются внутренними по отношению к операционной системе и могут изменяться от одного выпуска Windows к другому. Чтобы обеспечить совместимость приложения, лучше использовать общие функции, упомянутые в описании параметра *процессинформатионкласс* .

Если вы используете **звкуеринформатионпроцесс**, то получите доступ к функции через [динамическую компоновку во время выполнения](../dlls/using-run-time-dynamic-linking.md). Это дает коду возможность корректно реагировать, если функция была изменена или удалена из операционной системы. Однако изменения сигнатуры могут быть недоступны для обнаружения.

Эта функция не имеет связанной библиотеки импорта. Для динамической привязки к Ntdll.dll необходимо использовать функции [**LoadLibrary**](/windows/win32/api/libloaderapi/nf-libloaderapi-loadlibrarya) и [**GetProcAddress**](/windows/win32/api/libloaderapi/nf-libloaderapi-getprocaddress) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows \[Только классические приложения XP\]<br/>                                          |
| Минимальная версия сервера<br/> | Windows Только для \[ настольных приложений сервера 2003\]<br/>                                 |
| DLL<br/>                      | <dl> <dt>Ntdll.dll</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**чеккремотедебугжерпресент**](/windows/win32/api/debugapi/nf-debugapi-checkremotedebuggerpresent)
</dt> <dt>

[**GetProcessId**](/windows/win32/api/processthreadsapi/nf-processthreadsapi-getprocessid)
</dt> <dt>

[**исдебугжерпресент**](/windows/win32/api/debugapi/nf-debugapi-isdebuggerpresent)
</dt> <dt>

[**IsWow64Process**](/windows/win32/api/wow64apiset/nf-wow64apiset-iswow64process)
</dt> </dl>

 

 
