---
description: В этом разделе содержатся справочные сведения по структурам API видео Microsoft Direct3D 12.
ms.assetid: ''
title: Видеоструктуры Direct3D 12
ms.topic: article
ms.date: 06/03/2019
ms.openlocfilehash: dd73ba1cf374dade90963513ddbc92317cd3b05c
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127574938"
---
# <a name="direct3d-12-video-structures"></a>Видеоструктуры Direct3D 12

В этом разделе содержатся справочные сведения по структурам API видео Microsoft Direct3D 12.

## <a name="in-this-section"></a>В этом разделе

| Раздел                                                                                | Описание                                                                                              |
|---------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| [D3D12_FEATURE_DATA_VIDEO_DECODE_CONVERSION_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_decode_conversion_support)  | Возвращает список поддерживаемых профилей.|
| [D3D12_FEATURE_DATA_VIDEO_DECODE_FORMATS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_decode_formats)  | Возвращает список поддерживаемых форматов.|
| [D3D12_FEATURE_DATA_VIDEO_DECODE_HISTOGRAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_decode_histogram)  | Предоставляет данные для вызовов ID3D12VideoDevice:: Чеккфеатуресуппорт, когда заданный компонент имеет D3D12_FEATURE_VIDEO_DECODE_HISTOGRAM.|
| [D3D12_FEATURE_DATA_VIDEO_DECODE_PROFILES](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_decode_profiles)  | Возвращает список поддерживаемых профилей.|
| [D3D12_FEATURE_DATA_VIDEO_DECODE_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_decode_support)  | Извлекает сведения о поддержке для декодирования видео.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_CODEC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_codec)  | Извлекает значение, указывающее, поддерживается ли указанный кодек для кодирования видео.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_CODEC_CONFIGURATION_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_codec_configuration_support)  | Получает значение, указывающее, поддерживаются ли параметры поддержки указанного кодека для 
предоставленная конфигурация кодировки HEVC или извлекает поддерживаемую конфигурацию для кодирования H. 264.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_CODEC_PICTURE_CONTROL_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_codec_picture_control_support)  | Получает поддержку элемента управления "изображение" для указанного кодека и профиля.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_FRAME_SUBREGION_LAYOUT_MODE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_frame_subregion_layout_mode)  | Извлекает значение, указывающее, поддерживается ли для указанного режима макета подобласти фрейма указанный 
код, профиль и уровень.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_HEAP_SIZE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_heap_size)  | Извлекает значение, указывающее, поддерживается ли указанный кодек для кодирования видео, а также для значений на уровне 0 и 
Размеры L1 объекта кучи.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_INPUT_FORMAT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_input_format)  | Извлекает значение, указывающее, поддерживаются ли для кодирования видео указанный кодек, профиль и формат.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_INTRA_REFRESH_MODE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_intra_refresh_mode)  | Получает значение, указывающее, поддерживается ли заданный режим обновления для указанного кодека. 
профиль и уровень.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_OUTPUT_RESOLUTION](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_output_resolution)  | Возвращает список поддерживаемых разрешений для указанного кодека.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_OUTPUT_RESOLUTION_RATIOS_COUNT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_output_resolution_ratios_count)  | |
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_PROFILE_LEVEL](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_profile_level)  | Извлекает значение, указывающее, поддерживается ли указанный профиль для кодирования видео.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_RATE_CONTROL_MODE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_rate_control_mode)  | Извлекает значение, указывающее, поддерживается ли заданный режим управления скоростью для кодирования видео с помощью 
указанный кодек|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_RESOLUTION_SUPPORT_LIMITS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_resolution_support_limits)  | Представляет ограничения поддержки разрешения кодировщика видео для D3D12_FEATURE_DATA_VIDEO_ENCODER_SUPPORT 
дереве.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_RESOURCE_REQUIREMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_resource_requirements)  | Извлекает значения, указывающие требования к ресурсам для кодирования видео с указанной кодировкой 
узле.|
| [D3D12_FEATURE_DATA_VIDEO_ENCODER_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_encoder_support)  | Извлекает значения, указывающие поддержку для указанных функций кодирования видео и значений конфигурации.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMAND_COUNT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_command_count)  | Возвращает число команд расширения видео.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMAND_PARAMETER_COUNT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_command_parameter_count)  | Извлекает поддерживаемое количество параметров для указанного этапа параметра.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMAND_PARAMETERS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_command_parameters)  | Возвращает список параметров команды расширения видео для указанного этапа параметра.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMAND_SIZE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_command_size)  | Проверяет размер выделения для команды расширения видео.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMAND_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_command_support)  | Получает поддержку команды расширения видео с помощью определяемых командой входных и выходных структур.|
| [D3D12_FEATURE_DATA_VIDEO_EXTENSION_COMMANDS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_extension_commands)  | Возвращает список команд расширения видео из драйвера.|
| [D3D12_FEATURE_DATA_VIDEO_MOTION_ESTIMATOR](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_motion_estimator)  | Предоставляет данные для вызовов ID3D12VideoDevice:: Чеккфеатуресуппорт, когда заданный компонент имеет D3D12_FEATURE_VIDEO_MOTION_ESTIMATOR. Получает возможности оценки движения для кодировщика видео.|
| [D3D12_FEATURE_DATA_VIDEO_MOTION_ESTIMATOR_PROTECTED_RESOURCES](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_motion_estimator_protected_resources)  | Предоставляет данные для вызовов ID3D12VideoDevice:: Чеккфеатуресуппорт, когда заданный компонент имеет D3D12_FEATURE_VIDEO_MOTION_ESTIMATOR_PROTECTED_RESOURCES. Получает поддержку для оценки движения видео.|
| [D3D12_FEATURE_DATA_VIDEO_MOTION_ESTIMATOR_SIZE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_motion_estimator_size)  | Описывает размер выделения кучи для оценки движения видео.|
| [D3D12_FEATURE_DATA_VIDEO_PROCESS_MAX_INPUT_STREAMS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_process_max_input_streams)  | Возвращает максимальное число включенных потоков ввода, поддерживаемых обработчиком видео.|
| [D3D12_FEATURE_DATA_VIDEO_PROCESS_REFERENCE_INFO](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_process_reference_info)  | Извлекает число прошедших и будущих ссылочных кадров, необходимых для заданных режимов чередования, фильтрации, преобразования ставок или функций автоматической обработки.|
| [D3D12_FEATURE_DATA_VIDEO_PROCESS_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_feature_data_video_process_support)  | Предоставляет данные для вызовов ID3D12VideoDevice:: Чеккфеатуресуппорт, когда заданный компонент имеет D3D12_FEATURE_VIDEO_PROCESS_SUPPORT.|
| [D3D12_QUERY_DATA_VIDEO_DECODE_STATISTICS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_query_data_video_decode_statistics)  | Представляет данные для запроса статистики видеокодирования, вызываемого путем вызова ID3D12VideoDecodeCommandList:: Ендкуери.|
| [D3D12_RESOLVE_VIDEO_MOTION_VECTOR_HEAP_INPUT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_resolve_video_motion_vector_heap_input)  | Предоставляет входные данные для вызовов ID3D12VideoEncodeCommandList:: Ресолвемотионвекторхеап.|
| [D3D12_RESOLVE_VIDEO_MOTION_VECTOR_HEAP_OUTPUT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_resolve_video_motion_vector_heap_output)  | Получает выходные данные от вызовов ID3D12VideoEncodeCommandList:: Ресолвемотионвекторхеап.|
| [D3D12_RESOURCE_COORDINATE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_resource_coordinate)  | Описывает координаты ресурса.|
| [D3D12_VIDEO_DECODER_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decoder_desc)  | Описывает ID3D12VideoDecoder.|
| [D3D12_VIDEO_DECODER_HEAP_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decoder_heap_desc)  | Описывает ID3D12VideoDecoderHeap.|
| [D3D12_VIDEO_DECODE_COMPRESSED_BITSTREAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_compressed_bitstream)  | Представляет сжатый битовый поток, из которого декодировано видео.|
| [D3D12_VIDEO_DECODE_CONFIGURATION](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_configuration)  | Описывает конфигурацию видеодекодера.|
| [D3D12_VIDEO_DECODE_CONVERSION_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_conversion_arguments)  | Задает параметры для преобразования выходных данных декодирования.|
| [D3D12_VIDEO_DECODE_CONVERSION_ARGUMENTS1](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_conversion_arguments1)  | Задает параметры для преобразования выходных данных декодирования.|
| [D3D12_VIDEO_DECODE_FRAME_ARGUMENT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_frame_argument)  | Представляет параметры декодирования для кадра.|
| [D3D12_VIDEO_DECODE_INPUT_STREAM_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_input_stream_arguments)  | Задает параметры для входного потока для операции декодирования видео.|
| [D3D12_VIDEO_DECODE_OUTPUT_HISTOGRAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_output_histogram)  | Представляет выходной буфер гистограммы для одного компонента.|
| [D3D12_VIDEO_DECODE_OUTPUT_STREAM_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_output_stream_arguments)  | Задает параметры потока вывода для операции декодирования видео.|
| [D3D12_VIDEO_DECODE_OUTPUT_STREAM_ARGUMENTS1](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_output_stream_arguments1)  | Задает параметры потока вывода для операции декодирования видео.|
| [D3D12_VIDEO_DECODE_REFERENCE_FRAMES](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_reference_frames)  | Содержит список кадров ссылок для текущей операции декодирования.|
| [D3D12_VIDEO_DECODE_SUB_SAMPLE_MAPPING_BLOCK](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_decode_sub_sample_mapping_block)  | Определяет сопоставление байтов шифрования для вспомогательных примеров для декодирования видео.|
| [D3D12_VIDEO_ENCODE_REFERENCE_FRAMES](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encode_reference_frames)  | Представляет перестроенные образы ссылок для операции кодирования.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration)  | Представляет структуру конфигурации кодека для кодирования видео.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration_h264)  | Представляет конфигурацию кодека для кодировки H. 264.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration_hevc)  | Представляет конфигурацию кодека для кодирования HEVC.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration_support)  | Представляет структуру поддержки конфигурации кодеков для кодирования видео.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION_SUPPORT_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration_support_h264)  | Представляет поддержку конфигурации кодека кодировщика для кодирования H. 264.|
| [D3D12_VIDEO_ENCODER_CODEC_CONFIGURATION_SUPPORT_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_configuration_support_hevc)  | Представляет поддержку конфигурации кодека кодировщика для кодирования HEVC.|
| [D3D12_VIDEO_ENCODER_CODEC_PICTURE_CONTROL_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_picture_control_support)  | Представляет структуру поддержки элементов управления рисунка для нескольких кодеков.|
| [D3D12_VIDEO_ENCODER_CODEC_PICTURE_CONTROL_SUPPORT_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_picture_control_support_h264)  | Представляет параметры поддержки элемента управления "изображение" для кодирования видео H. 264.|
| [D3D12_VIDEO_ENCODER_CODEC_PICTURE_CONTROL_SUPPORT_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_codec_picture_control_support_hevc)  | Представляет параметры поддержки элемента управления "изображение" для кодирования видео HEVC.|
| [D3D12_VIDEO_ENCODER_COMPRESSED_BITSTREAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_compressed_bitstream)  | Инкапсулирует сжатый выходной битовый поток для операции кодирования.|
| [D3D12_VIDEO_ENCODER_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_desc)  | Описывает ID3D12VideoEncoder.|
| [D3D12_VIDEO_ENCODER_ENCODE_OPERATION_METADATA_BUFFER](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_encode_operation_metadata_buffer)  | Представляет буфер, содержащий метаданные об операции ID3D12VideoEncodeCommandList2:: Енкодефраме.|
| [D3D12_VIDEO_ENCODER_ENCODEFRAME_INPUT_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_encodeframe_input_arguments)  | Представляет входные аргументы для ID3D12VideoEncodeCommandList2:: Енкодефраме.|
| [D3D12_VIDEO_ENCODER_ENCODEFRAME_OUTPUT_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_encodeframe_output_arguments)  | Представляет выходные аргументы для ID3D12VideoEncodeCommandList2:: Енкодефраме.|
| [D3D12_VIDEO_ENCODER_FRAME_SUBREGION_METADATA](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_frame_subregion_metadata)  | Представляет метаданные подобласти видеокодировщика.|
| [D3D12_VIDEO_ENCODER_HEAP_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_heap_desc)  | Описывает ID3D12VideoEncoderHeap.|
| [D3D12_VIDEO_ENCODER_INTRA_REFRESH](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_intra_refresh)  | Представляет параметры обновления для кодирования видео.|
| [D3D12_VIDEO_ENCODER_LEVEL_SETTING](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_level_setting)  | Представляет настройку уровня кодировщика видео.|
| [D3D12_VIDEO_ENCODER_LEVEL_TIER_CONSTRAINTS_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_level_tier_constraints_hevc)  | Связывает уровень и уровень для настройки параметров уровня высокопроизводительного видео (HEVC).|
| [D3D12_VIDEO_ENCODER_OUTPUT_METADATA](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_output_metadata)  | Представляет метаданные об операции ID3D12VideoEncodeCommandList2:: Енкодефраме.|
| [D3D12_VIDEO_ENCODER_OUTPUT_METADATA_STATISTICS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_output_metadata_statistics)  | Представляет статистику кодирования для операции ID3D12VideoEncodeCommandList2:: Енкодефраме.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_CODEC_DATA](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_codec_data)  | Представляет элементы управления уровня изображения для связанной команды Енкодефраме для нескольких кодеков.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_CODEC_DATA_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_codec_data_h264)  | Представляет элементы управления уровня изображения для связанной команды Енкодефраме для кодировки H. 264.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_CODEC_DATA_H264_REFERENCE_PICTURE_LIST_MODIFICATION_OPERATION](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_codec_data_h264_reference_picture_list_modification_operation)  | Представляет операцию изменения списка изображений для кодирования видео H264 Single bitrate.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_CODEC_DATA_H264_REFERENCE_PICTURE_MARKING_OPERATION](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_codec_data_h264_reference_picture_marking_operation)  | Описывает изменения в ссылках на рисунки как на операции с памятью в виде кортежа операции идентификатор 
и связанные параметры, необходимые для операции.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_CODEC_DATA_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_codec_data_hevc)  | Представляет элементы управления уровня изображения для связанной команды Енкодефраме для кодировки HEVC.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_desc)  | 06/30/2021|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_SUBREGIONS_LAYOUT_DATA](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_subregions_layout_data)  | Определяет подобласти элемента управления рисунка как срезы для нескольких кодеков.|
| [D3D12_VIDEO_ENCODER_PICTURE_CONTROL_SUBREGIONS_LAYOUT_DATA_SLICES](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_control_subregions_layout_data_slices)  | Определяет подобласти как срезы для кодеков, поддерживающих этот режим секционирования.|
| [D3D12_VIDEO_ENCODER_PICTURE_RESOLUTION_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_resolution_desc)  | Определяет разрешение изображения кодировщика видео.|
| [D3D12_VIDEO_ENCODER_PICTURE_RESOLUTION_RATIO_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_picture_resolution_ratio_desc)  | Определяет отношение разрешения в виде дробной части ирредуЦибле.|
| [D3D12_VIDEO_ENCODER_PROFILE_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_profile_desc)  | Описывает профиль кодировщика.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control)  | Представляет конфигурацию управления скоростью видеодекодера.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL_CBR](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control_cbr)  | Представляет определение структуры управления скоростью для режима постоянной скорости.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL_CONFIGURATION_PARAMS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control_configuration_params)  | Представляет Управление частотой видеокодировщика определения структуры для D3D12_VIDEO_ENCODER_RATE_CONTROL 
дереве.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL_CQP](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control_cqp)  | Представляет определение структуры управления скоростью для постоянного режима параметров дискретизация.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL_QVBR](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control_qvbr)  | Представляет определение структуры управления скоростью для целевого объекта качества постоянного с ограниченной скоростью.|
| [D3D12_VIDEO_ENCODER_RATE_CONTROL_VBR](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_rate_control_vbr)  | Представляет определение структуры управления скоростью для режима с переменной скоростью.|
| [D3D12_VIDEO_ENCODER_RECONSTRUCTED_PICTURE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_reconstructed_picture)  | Представляет пересозданное изображение из входного кадра, переданного в операцию кодирования.|
| [D3D12_VIDEO_ENCODER_REFERENCE_PICTURE_DESCRIPTOR_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_reference_picture_descriptor_h264)  | Представляет дескриптор изображения ссылки для кодирования видео H. 264.|
| [D3D12_VIDEO_ENCODER_REFERENCE_PICTURE_DESCRIPTOR_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_reference_picture_descriptor_hevc)  | Представляет дескриптор изображения ссылки для кодирования видео HEVC.|
| [D3D12_VIDEO_ENCODER_RESOLVE_METADATA_INPUT_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_resolve_metadata_input_arguments)  | Представляет входные аргументы для вызова ID3D12VideoEncodeCommandList2:: Ресолвинкодераутпутметадата.|
| [D3D12_VIDEO_ENCODER_RESOLVE_METADATA_OUTPUT_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_resolve_metadata_output_arguments)  | Представляет выходные аргументы для вызова ID3D12VideoEncodeCommandList2:: Ресолвинкодераутпутметадата.|
| [D3D12_VIDEO_ENCODER_SEQUENCE_CONTROL_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_sequence_control_desc)  | |
| [D3D12_VIDEO_ENCODER_SEQUENCE_GOP_STRUCTURE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_sequence_gop_structure)  | Представляет структуру GOP для нескольких видеокодеков.|
| [D3D12_VIDEO_ENCODER_SEQUENCE_GOP_STRUCTURE_H264](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_sequence_gop_structure_h264)  | Представляет структуру GOP для кодирования видео H. 264.|
| [D3D12_VIDEO_ENCODER_SEQUENCE_GOP_STRUCTURE_HEVC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_encoder_sequence_gop_structure_hevc)  | Представляет структуру GOP для кодирования видео HEVC.|
| [D3D12_VIDEO_EXTENSION_COMMAND_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_extension_command_desc)  | Описывает команду расширения видео.|
| [D3D12_VIDEO_EXTENSION_COMMAND_INFO](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_extension_command_info)  | Описывает команду расширения видео.|
| [D3D12_VIDEO_EXTENSION_COMMAND_PARAMETER_INFO](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_extension_command_parameter_info)  | Описывает параметр команды расширения видео.|
| [D3D12_VIDEO_FORMAT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_format)  | Определяет сочетание формата пикселей и цветового пространства для описания содержимого ресурса.|
| [D3D12_VIDEO_MOTION_ESTIMATOR_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_motion_estimator_desc)  | Описывает ID3D12VideoMotionEstimator. Передайте эту структуру в ID3D12VideoDevice1:: Креатевидеомотионестиматор, чтобы создать экземпляр ID3D12VideoMotionEstimator.|
| [D3D12_VIDEO_MOTION_ESTIMATOR_INPUT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_motion_estimator_input)  | Предоставляет входные данные для вызовов ID3D12VideoEncodeCommandList:: Естиматемотион.|
| [D3D12_VIDEO_MOTION_ESTIMATOR_OUTPUT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_motion_estimator_output)  | Получает выходные данные от вызовов ID3D12VideoEncodeCommandList:: Естиматемотион.|
| [D3D12_VIDEO_MOTION_VECTOR_HEAP_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_motion_vector_heap_desc)  | Описывает ID3D12VideoMotionEstimatorHeap. Передайте эту структуру в ID3D12VideoDevice1:: Креатевидеомотионестиматорхеап, чтобы создать экземпляр ID3D12VideoMotionEstimatorHeap.|
| [D3D12_VIDEO_PROCESS_ALPHA_BLENDING](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_alpha_blending)  | Задает параметры альфа-смешения для обработки видео.|
| [D3D12_VIDEO_PROCESS_FILTER_RANGE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_filter_range)  | Определяет диапазон поддерживаемых значений для фильтра изображений.|
| [D3D12_VIDEO_PROCESS_INPUT_STREAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_input_stream)  | Содержит входные данные для функции смешения видео процессора.|
| [D3D12_VIDEO_PROCESS_INPUT_STREAM_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_input_stream_arguments)  | Указывает входные аргументы потока для входного потока, переданного в ID3D12VideoCommandList::P Роцессфрамес.|
| [D3D12_VIDEO_PROCESS_INPUT_STREAM_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_input_stream_desc)  | Задает параметры для входного потока для операции обработки видео.|
| [D3D12_VIDEO_PROCESS_INPUT_STREAM_RATE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_input_stream_rate)  | Предоставляет сведения о частоте потока.|
| [D3D12_VIDEO_PROCESS_LUMA_KEY](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_luma_key)  | Задает параметры, используемые для ключа яркости.|
| [D3D12_VIDEO_PROCESS_OUTPUT_STREAM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_output_stream)  | Представляет поток вывода для команд обработки видео.|
| [D3D12_VIDEO_PROCESS_OUTPUT_STREAM_ARGUMENTS](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_output_stream_arguments)  | Указывает выходные аргументы потока для выходных данных, переданных в ID3D12VideoCommandList::P Роцессфрамес.|
| [D3D12_VIDEO_PROCESS_OUTPUT_STREAM_DESC](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_output_stream_desc)  | Указывает выходные аргументы потока для выходных данных, переданных в ID3D12VideoProcessCommandList::P Роцессфрамес.|
| [D3D12_VIDEO_PROCESS_REFERENCE_SET](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_reference_set)  | Содержит справочные кадры, необходимые для обработки видео.|
| [D3D12_VIDEO_PROCESS_TRANSFORM](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_process_transform)  | Задает параметры преобразования для обработки видео.|
| [D3D12_VIDEO_SAMPLE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_sample)  | Описывает ширину, высоту, формат и цветовую область буфера изображения.|
| [D3D12_VIDEO_SCALE_SUPPORT](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_scale_support)  | Описание поддерживаемого диапазона масштабирования для размера выходных данных для масштабируемого видео.|
| [D3D12_VIDEO_SIZE_RANGE](/windows/desktop/api/d3d12video/ns-d3d12video-d3d12_video_size_range)  | Описывает диапазон поддерживаемых размеров для масштабируемого видео.|



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[API-интерфейсы видео Direct3D 12](direct3d-12-video-apis.md)
</dt> </dl>

 

 



