---
description: Декодер Dolby Audio — это MFT, декодированное в формате Dolby Digital (AC-3) и Dolby Digital Plus.
ms.assetid: A968914A-E4C5-4472-8776-C73F5910089A
title: Декодер Dolby Audio
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: 1ae38516edd935def5d9b2b041c942a729c45c61
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122479870"
---
# <a name="dolby-audio-decoder"></a>Декодер Dolby Audio

Декодер Dolby Audio — это [Media Foundation преобразование](media-foundation-transforms.md) (MFT), которое декодирует следующие типы потоков:

-   Dolby Digital, также называемая Dolby AC-3
-   Dolby Digital Plus, также называемый расширенным AC-3 (E-AC-3)

> [!IMPORTANT]
> для версий Windows, выпущенных до Windows 8, реализация технологии dolby digital в корпорации майкрософт ограничена условиями программы цифрового лицензирования dolby, используемой приложениями майкрософт.

 

Дополнительные сведения об этих форматах см. в документе по расширенному телевидению *цифрового звука (AC-3, E-AC-3) версии B*.

Декодер также может преобразовать поток Dolby Digital Plus в цифровой формат Dolby для вывода AC-3 S/ПИДФ или отформатировать поток Dolby Digital Plus для цифрового выхода HDMI.

## <a name="class-identifier"></a>Идентификатор класса

Идентификатором класса (CLSID) декодера Dolby Audio является **CLSID \_ кмсддплусдекмфт**, определенный в файле заголовка вмкодекдсп. h.

## <a name="input-types"></a>Типы входных данных

Декодер Dolby Audio поддерживает следующие входные подтипы.



| Subtype                                 | Описание                                                                                                                                                 | Header       |
|-----------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------|
| **МЕДИАСУБТИПЕ \_ Dolby \_ AC3**            | Dolby Digital Audio.                                                                                                                                        | мфапи. h      |
| **МЕДИАСУБТИПЕ \_ DVM**                   | Dolby Digital Audio; см. раздел [**аудио подтипы**](../directshow/audio-subtypes.md). Этот подтип можно использовать взаимозаменяемым с **медиасубтипе \_ Dolby \_ AC3**.<br/> | вмкодекдсп. h |
| **Мфаудиоформат \_ Dolby \_ Digital \_ Plus** | Dolby Digital Plus Audio.                                                                                                                                   | мфапи. h      |



 

В следующей таблице перечислены необходимые и необязательные атрибуты для входного типа носителя.




| attribute | Описание | Remarks | 
|-----------|-------------|---------|
| <a href="mf-mt-major-type-attribute.md">MF_MT_MAJOR_TYPE</a> | Основной тип. | Обязательный. Необходимо <strong>MFMediaType_Audio</strong>. | 
| <a href="mf-mt-subtype-attribute.md">MF_MT_SUBTYPE</a> | Подтип аудио. | Обязательный. Дополнительные сведения см. в предыдущей таблице. | 
| <a href="mf-mt-audio-samples-per-second-attribute.md">MF_MT_AUDIO_SAMPLES_PER_SECOND</a> | Частота выборки, в примерах в секунду. | Необязательный элемент. Допустимые значения: 48000, 44100, 32000, 24000, 22050 и 16000. Если этот атрибут не задан, по умолчанию используется значение 48000. <br /><blockquote>[!Note]<br />Потоки Dolby AC-3 ограничиваются тремя самыми высокими тарифами в этом списке.</blockquote><br /> | 
| <a href="mf-mt-audio-num-channels-attribute.md">MF_MT_AUDIO_NUM_CHANNELS</a> | Количество каналов, включая канал с низкой частотой (НИЗКОЧАСТОТный), если он есть. | Необязательный элемент. Допустимые значения находятся в диапазоне от 1 (моно) до 8 (Конфигурация канала 7,1). Если этот атрибут не задан, по умолчанию используется значение 2 (стерео). | 
| <a href="mf-mt-audio-channel-mask-attribute.md">MF_MT_AUDIO_CHANNEL_MASK</a> | Указывает назначение звуковых каналов для позиционирования динамиков. | Необязательный элемент. Если указано, значение должно соответствовать числу звуковых каналов. Если атрибут не задан, декодер использует маску канала по умолчанию на основе числа каналов. | 




 

В следующей таблице перечислены поддерживаемые конфигурации канала Dolby.




| Конфигурация канала | Число каналов | Маски каналов | 
|-----------------------|--------------------|---------------|
| 1/0 (моно) | 1 | 0x4 (<strong>SPEAKER_FRONT_CENTER</strong>) | 
| 2/0 (стерео) или 1 + 1 (два Mono) | 2 | 0x3 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong>) | 
| 3/0 | 3 | 0x7 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | SPEAKER_FRONT_CENTER) | 
| 2/1 | 3 | 0x103 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_BACK_CENTER</strong>) | 
| 3/1 | 4 | 0x107 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_BACK_CENTER</strong>) | 
| 2/2 | 4 | 0x33 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_BACK_LEFT</strong> | <strong>SPEAKER_BACK_RIGHT</strong>)<br /> или<br /> 0x603 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_SIDE_LEFT</strong> | <strong>SPEAKER_SIDE_RIGHT</strong>) <br /> | 
| 3/2 | 5 | 0x37 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_BACK_LEFT</strong> | <strong>SPEAKER_BACK_RIGHT</strong>)<br /> или<br /> 0x607 (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_SIDE_LEFT</strong> | <strong>SPEAKER_SIDE_RIGHT</strong>) <br /> | 
| 3/2 + НИЗКОЧАСТОТНЫЙ | 6 | 0x3F (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_LOW_FREQUENCY</strong> | <strong>SPEAKER_BACK_LEFT</strong> | <strong>SPEAKER_BACK_RIGHT</strong>)<br /> или<br /> 0x60F (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_LOW_FREQUENCY</strong> | <strong>SPEAKER_SIDE_LEFT</strong> | <strong>SPEAKER_SIDE_RIGHT</strong>)<br /> | 
| 3/2/2 + НИЗКОЧАСТОТНЫЙ<blockquote>[!Note]<br />Только Dolby Digital Plus.</blockquote><br /><br /> | 8 | 0x63F (<strong>SPEAKER_FRONT_LEFT</strong> | <strong>SPEAKER_FRONT_RIGHT</strong> | <strong>SPEAKER_FRONT_CENTER</strong> | <strong>SPEAKER_LOW_FREQUENCY</strong> | <strong>SPEAKER_BACK_LEFT</strong> | <strong>SPEAKER_BACK_RIGHT</strong> | SPEAKER_SIDE_LEFT | SPEAKER_SIDE_RIGHT) | 




 

Кроме того, конфигурации каналов 1/0, 2/0, 3/0, 2/1, 3/1 и 2/2 также могут отображаться с каналом НИЗКОЧАСТОТного канала.

## <a name="output-types"></a>Типы вывода

Декодер Dolby Audio поддерживает следующие выходные типы выходных данных.



| Subtype                                                   | Описание                                                                                                                               | Header    |
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|-----------|
| **Мфаудиоформат \_ Dolby \_ AC3 \_ SPDIF**                      | Звук Dolby AC-3, отформатированный для цифрового выхода S/PDIF.                                                                                     | мфапи. h   |
| **\_ПОДТИП ксдатаформат \_ IEC61937 \_ Dolby \_ Digital \_ Plus** | Dolby Digital Plus Audio, форматированный для цифрового выхода HDMI.                                                                               | ксмедиа. h |
| **Мфаудиоформат \_ float**                                  | IEEE 32-разрядный звук PCM с плавающей точкой<br/> **Windows 10**: стерео, 5,1, 7,1<br/> **Предыдущие версии**: стерео, 5,1<br/> | мфапи. h   |
| **Мфаудиоформат \_ PCM**                                    | 16-разрядный звук PCM<br/> **Windows 10**: стерео, 5,1, 7,1<br/> **Предыдущие версии**: стерео, 5,1<br/>                     | мфапи. h   |



 

В следующей таблице перечислены обязательные и необязательные атрибуты для выходного типа мультимедиа.




| attribute | Описание | Remarks | 
|-----------|-------------|---------|
| <a href="mf-mt-major-type-attribute.md">MF_MT_MAJOR_TYPE</a> | Основной тип. | Обязательный. Необходимо <strong>MFMediaType_Audio</strong>. | 
| <a href="mf-mt-subtype-attribute.md">MF_MT_SUBTYPE</a> | Подтип аудио. | Обязательный. Дополнительные сведения см. в предыдущей таблице. | 
| <a href="mf-mt-audio-samples-per-second-attribute.md">MF_MT_AUDIO_SAMPLES_PER_SECOND</a> | Частота выборки, в примерах в секунду. | Обязательный. Допустимые значения: 48000, 44100, 32000, 24000, 22050 и 16000. Частота выборки выходных данных должна совпадать с частотой выборки данных. Декодер не может изменить частоту выборки потока. | 
| <a href="mf-mt-audio-num-channels-attribute.md">MF_MT_AUDIO_NUM_CHANNELS</a> | Количество каналов, включая канал с низкой частотой (НИЗКОЧАСТОТный), если он есть. | Требуется для выходных данных PCM. <br /> Не требуется для цифрового вывода. <br /> Если входной тип — моно, стерео или Dual-Mono (все без канала НИЗКОЧАСТОТного звучания), единственное допустимое значение — 2 для стерео Output. В противном случае значение может быть следующим: <br /><ul><li>2 для стерео довнмикс</li><li>6 для конфигураций каналов 5,1</li><li>8 для конфигураций каналов 7,1</li></ul> | 
| <a href="mf-mt-audio-channel-mask-attribute.md">MF_MT_AUDIO_CHANNEL_MASK</a> | Указывает назначение звуковых каналов для позиционирования динамиков. | Требуется для вывода PCM, если число каналов больше 2. Значение должно быть следующим:<br /><ul><li>0x3 для стерео вывода</li><li>0x3F для выходных данных канала 5,1</li><li>0x63F для выходных данных канала 7,1</li></ul>Не требуется для цифрового вывода. <br /> | 
| <a href="mf-mt-audio-bits-per-sample-attribute.md">MF_MT_AUDIO_BITS_PER_SAMPLE</a> | Число битов на аудио выборка. | Требуется для выходных данных PCM. Значение должно быть 32 для <strong>MFAudioFormat_Float</strong>и 16 для <strong>MFAudioFormat_PCM</strong>.<br /> Не требуется для цифрового вывода.<br /> | 
| <a href="mf-mt-audio-valid-bits-per-sample-attribute.md">MF_MT_AUDIO_VALID_BITS_PER_SAMPLE</a> | Количество допустимых битов звуковых данных в каждом звуковом примере. | Необязательно для выходных данных PCM. Если значение задано, оно должно быть идентично значению <a href="mf-mt-audio-bits-per-sample-attribute.md">MF_MT_AUDIO_BITS_PER_SAMPLE</a>.<br /> Не требуется для подтипов цифровых выходных данных.<br /> | 
| <a href="mf-mt-audio-block-alignment-attribute.md">MF_MT_AUDIO_BLOCK_ALIGNMENT</a> | Выравнивание блокировки в байтах. | Необязательно для выходных данных PCM. Не требуется для цифрового вывода. | 
| <a href="mf-mt-audio-avg-bytes-per-second-attribute.md">MF_MT_AUDIO_AVG_BYTES_PER_SECOND</a> | Среднее число байтов в секунду. | Необязательно для выходных данных PCM. Не требуется для цифрового вывода. | 




 

## <a name="transform-attributes"></a>Атрибуты преобразования

Декодер Dolby Audio реализует метод [**имфтрансформ:: OutAttribute**](/windows/desktop/api/mftransform/nf-mftransform-imftransform-getattributes) . Приложение может использовать этот метод для получения или установки следующих атрибутов.



| attribute                                                                                | Описание                                                                                                                                                                                                                                                                              |
|------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [КОДЕКАПИ \_ авдекаудиодуалмоно](../directshow/avdecaudiodualmono-property.md)                        | Указывает, кодируется ли звуковой поток Dolby из 2 каналов в формате стерео или Dual-Mono. Перед декодированием первого кадра Dolby значение **еавдекаудиодуалмоно не \_ указано**. После декодирования значение отражает самый последний кадр Dolby.<br/> Только для чтения. <br/> |
| [КОДЕКАПИ \_ авдекаудиодуалмонорепромоде](../directshow/avdecaudiodualmonorepromode-property.md)      | Указывает, как декодер воссоздает аудио-файлы с двумя моноями. По умолчанию используется значение **еавдекаудиодуалмонорепромоде \_ Left \_ Mono**. Приложение может установить это свойство в любое время.<br/> Read/write.<br/>                                                                            |
| [КОДЕКАПИ \_ авдеккоммонмеанбитрате](../directshow/avdeccommonmeanbitrate.md)                         | Для потоков Dolby Digital (AC-3) указывает скорость потока входных потоков в битах в секунду. Для Dolby Digital Plus (E-AC3) значение всегда равно нулю.<br/> Только для чтения.<br/>                                                                                              |
| [КОДЕКАПИ \_ авдекдддинамикранжескалехигх](../directshow/avdecdddynamicrangescalehigh-property.md)    | Высокоуровневая вырезание, когда декодер выполняет динамическое управление диапазонами.<br/> Read/write.<br/>                                                                                                                                                                                    |
| [КОДЕКАПИ \_ авдекдддинамикранжескалелов](../directshow/avdecdddynamicrangescalelow-property.md)      | Низкоуровневые улучшения, когда декодер выполняет динамический контроль диапазона.<br/> Read/write.<br/>                                                                                                                                                                                   |
| [КОДЕКАПИ \_ авдекддоператионалмоде](../directshow/avdecddoperationalmode-property.md)                | Режим управления сжатием.<br/> Read/write.<br/>                                                                                                                                                                                                                          |
| [КОДЕКАПИ \_ авдекддстереодовнмиксмоде](codecapi-avdecddstereodownmixmode.md)              | Тип стерео довнмикс. Это свойство применяется, если входные данные являются многоканальным потоком, а выходные данные — стерео потоком.<br/> Read/write.<br/>                                                                                                                           |
| [Основная таблица MFT \_ поддерживает \_ \_ изменение динамического формата \_](mft-support-dynamic-format-change-attribute.md) | Этот атрибут возвращает **значение false**, указывающее, что декодер должен быть остановлен до установки нового входного типа.<br/> Read/write.<br/>                                                                                                                                          |



 

## <a name="remarks"></a>Комментарии

Декодер принимает только необработанные потоки Dolby, как определено параметром/52B. полезные данные, такие как пакетированные простые Потоки (PES), не поддерживаются. Для Dolby Digital Plus декодер декодировать до 5,1 каналов. в Windows 10 потоки каналов 7,1 декодированы без довнмикс. В предыдущих версиях ОС, если поток 7,1 каналов, будет декодирован только довнмикс-канал 5,1. Если поток — Dolby Digital Plus с более чем одним независимым подпотоком, декодирован только независимый подпоток 0. Декодер пропускает другие независимые подпотоки. Кроме того, декодер пропускает все зависимые подпотоки. Декодер поддерживает расшифровку и декодирование потоков, защищенных с помощью технологии Digital Rights Management (DRM).

Если тип входного носителя имеет конфигурацию канала, отличную от Mono, стерео или Dual-Mono (без канала НИЗКОЧАСТОТного звучания), декодер предоставляет два варианта конфигураций выходного канала:

-   8-канальный вывод (Конфигурация канала 7,1)
-   6-канальный вывод (Конфигурация канала 5,1)
-   Стерео довнмикс

Если выбрано стерео довнмикс, то тип довнмикс можно задать в MFT с помощью свойства [кодекапи \_ авдекддстереодовнмиксмоде](codecapi-avdecddstereodownmixmode.md) .

Если тип выходных данных — **мфаудиоформат \_ Dolby \_ AC3 \_ SPDIF**, то каждый выходной буфер содержит 6 144 байт. Буфер начинается с 8-байтового заголовка S/PDIF, за которым следует сжатый кадр AC-3, за которым следует ноль заполнения до 6 144 байт.

Если тип выходных данных — **ксдатаформат подтип \_ \_ IEC61937 \_ Dolby \_ Digital \_ PLUS**, каждый выходной буфер содержит 24 576 байт. Буфер начинается с 8-байтового заголовка S/PDIF, за которым следуют 1 – 6 сжатые кадры Dolby Digital Plus, соответствующие примерам PCM 1 536, за которыми следует ноль заполнения до 24 576 байт. Для выходных данных HDMI упаковывается только независимый подпоток 0.

Таблица MFT декодера зарегистрирована с флагом **\_ перечисления MFT Enum \_ \_ фиелдофусе**, который указывает, что Таблица MFT, которая должна быть разблокирована приложением перед использованием. Дополнительные сведения см. в разделе [ограничения использования](field-of-use-restrictions.md).

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|--------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 8 \[ приложения UWP для классических приложений \|\]<br/>                                          |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                  |
| DLL<br/>                      | <dl> <dt>Msauddecmft.dll</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[Объекты кодека](codecobjects.md)
</dt> </dl>

 

 
