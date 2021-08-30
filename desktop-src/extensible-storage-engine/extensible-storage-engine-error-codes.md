---
description: дополнительные сведения о расширенных кодах ошибок служба хранилища Engine
title: коды ошибок расширенного механизма служба хранилища
TOCTitle: Extensible Storage Engine Error Codes
ms:assetid: 7534370d-aed6-4980-b1ca-c3d063507e31
ms:mtpsurl: https://msdn.microsoft.com/library/Gg269297(v=EXCHG.10)
ms:contentKeyID: 32765589
ms.date: 09/22/2016
ms.topic: reference
api_name: ''
topic_type:
- apiref
- kbArticle
api_type:
- COM
api_location: ''
ROBOTS: INDEX,FOLLOW
ms.openlocfilehash: cdbdff7255b621eaab59cfbf38cb577a6e8c0331
ms.sourcegitcommit: 9b5faa61c38b2d0c432b7f2dbee8c127b0e28a7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2021
ms.locfileid: "122481780"
---
# <a name="extensible-storage-engine-error-codes"></a>коды ошибок расширенного механизма служба хранилища


_**Применимо к:** Windows | Windows Сервером_

## <a name="extensible-storage-engine-error-codes"></a>коды ошибок расширенного механизма служба хранилища

следующие коды ошибок (flags) используются функциями в расширенном API-интерфейсе служба хранилища Engine.

Значение [JET_ERR](./jet-err.md) , равное нулю, должно интерпретироваться как Success.


| <p>Успешное завершение</p> | <p>Описание</p> | 
|----------------|--------------------|
| <p>JET_errSuccess 0</p> | <p>Функция выполнена успешно.</p> | 



Значение [JET_ERR](./jet-err.md) , большее нуля, должно интерпретироваться как предупреждение.


| <p>Предупреждения</p> | <p>Описание</p> | 
|-----------------|--------------------|
| <p>JET_wrnRemainingVersions<br />321</p> | <p>Хранилище версий все еще активно. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_wrnUniqueKey<br />345</p> | <p>Поиск в неуникальном индексе подает уникальный ключ. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_wrnSeparateLongValue<br />406</p> | <p>Столбец базы данных имеет разделенное длинное значение. Эта ошибка возвращается диспетчером записей.</p> | 
| <p>JET_wrnExistingLogFileHasBadSignature<br />558</p> | <p>Существующий файл журнала имеет неправильную подпись.</p> | 
| <p>JET_wrnExistingLogFileIsNotContiguous<br />559</p> | <p>Существующий файл журнала не является смежным.</p> | 
| <p>JET_wrnSkipThisRecord<br />564</p> | <p>Эта ошибка относится только к внутреннему использованию.</p> | 
| <p>JET_wrnTargetInstanceRunning<br />578</p> | <p>TargetInstance, указанный для восстановления, работает.</p> | 
| <p>JET_wrnDatabaseRepaired<br />595</p> | <p>Повреждение базы данных восстановлено.</p> | 
| <p>JET_wrnColumnNull<br />1004</p> | <p>Столбец имеет значение <strong>null</strong> .</p> | 
| <p>JET_wrnBufferTruncated<br />1006</p> | <p>Буфер слишком мал для данных.</p> | 
| <p>JET_wrnDatabaseAttached<br />1007</p> | <p>База данных уже присоединена.</p> | 
| <p>JET_wrnSortOverflow<br />1009</p> | <p>Для выполнения сортировки не хватает памяти.</p> | 
| <p>JET_wrnSeekNotEqual<br />1039</p> | <p>Точное совпадение не найдено во время поиска.</p> | 
| <p>JET_wrnRecordFoundGreater<br />JET_wrnSeekNotEqual</p> | <p>Точное совпадение не найдено во время поиска. Эта ошибка возвращается диспетчером записей.</p> | 
| <p>JET_wrnRecordFoundLess<br />JET_wrnSeekNotEqual</p> | <p>Точное совпадение не найдено во время поиска. Эта ошибка возвращается диспетчером записей.</p> | 
| <p>JET_wrnNoErrorInfo<br />1055</p> | <p>Расширенные сведения об ошибках отсутствуют.</p> | 
| <p>JET_wrnNoIdleActivity<br />1058</p> | <p>Неактивное действие не выполнено.</p> | 
| <p>JET_wrnNoWriteLock<br />1067.</p> | <p>Отсутствует блокировка записи на уровне транзакций 0.</p> | 
| <p>JET_wrnColumnSetNull<br />1068</p> | <p>Для столбца задается значение <strong>null</strong> .</p> | 
| <p>JET_wrnTableEmpty<br />1301</p> | <p>Была открыта пустая таблица.</p> | 
| <p>JET_wrnTableInUseBySystem<br />1327</p> | <p>Для очистки системы в таблице открыт курсор.</p> | 
| <p>JET_wrnCorruptIndexDeleted<br />1415</p> | <p>Неактуальный индекс должен быть удален.</p> | 
| <p>JET_wrnColumnMaxTruncated<br />1512</p> | <p>Максимальная длина слишком велика и была усечена.</p> | 
| <p>JET_wrnCopyLongValue<br />1520</p> | <p>Значение большого двоичного объекта было перемещено из записи в отдельное хранилище больших двоичных объектов.</p><p><strong>Примечание</strong> . Эта ошибка относится только к внутреннему использованию.</p> | 
| <p>JET_wrnColumnSkipped<br />1531</p> | <p>Значения столбца не были возвращены, так как соответствующий идентификатор столбца или элемент <em>итагсекуенце</em> из структуры <a href="gg294052(v=exchg.10).md">JET_ENUMCOLUMNVALUE</a> , запрошенной для перечисления, имел значение null.</p> | 
| <p>JET_wrnColumnNotLocal<br />1532</p> | <p>Значения столбца не были возвращены, так как их не удалось перестроить из существующих данных.</p> | 
| <p>JET_wrnColumnMoreTags<br />1533</p> | <p>Существующие значения столбца не были запрошены для перечисления.</p> | 
| <p>JET_wrnColumnTruncated<br />1534</p> | <p>Значение столбца было усечено по запрошенному пределу размера во время перечисления.</p> | 
| <p>JET_wrnColumnPresent<br />1535</p> | <p>Значения столбца существуют, но не возвращены запросом.</p> | 
| <p>JET_wrnColumnSingleValue<br />1536</p> | <p>Значение столбца было возвращено в JET_COLUMNENUM в результате задания JET_bitEnumerateCompressOutput.</p> | 
| <p>JET_wrnColumnDefault<br />1537</p> | <p>Значение столбца устанавливается в значение по умолчанию для столбца.</p> | 
| <p>JET_wrnDataHasChanged<br />1610</p> | <p>Данные были изменены.</p> | 
| <p>JET_wrnKeyChanged<br />1618</p> | <p>Используется новый ключ.</p> | 
| <p>JET_wrnFileOpenReadOnly<br />1813</p> | <p>Файл базы данных доступен только для чтения.</p> | 
| <p>JET_wrnIdleFull<br />1908</p> | <p>Неактивный реестр заполнен.</p> | 
| <p>JET_wrnDefragAlreadyRunning<br />2000</p> | <p>В указанной базе данных уже запущена оперативная дефрагментация.</p> | 
| <p>JET_wrnDefragNotRunning<br />2001</p> | <p>В указанной базе данных не запущена оперативная дефрагментация.</p> | 
| <p>JET_wrnCallbackNotRegistered<br />2100</p> | <p>Регистрация несуществующей функции обратного вызова отменена.</p> | 



Значение [JET_ERR](./jet-err.md) , меньшее нуля, должно интерпретироваться как ошибка.


| <p>ошибки</p> | <p>Описание</p> | 
|---------------|--------------------|
| <p>JET_wrnNyi<br />-1</p> | <p>Функция еще не реализована.</p> | 
| <p>JET_errRfsFailure<br />–100</p> | <p>Не удалось выполнить симулятор сбоя ресурса.</p> | 
| <p>JET_errRfsNotArmed<br />–101</p> | <p>Симулятор сбоя ресурса не инициализирован.</p> | 
| <p>JET_errFileClose<br />–102</p> | <p>Не удалось закрыть файл.</p> | 
| <p>JET_errOutOfThreads<br />-103</p> | <p>Не удалось запустить поток.</p> | 
| <p>JET_errTooManyIO<br />-105</p> | <p>Система занята из-за слишком большого количества IOs.</p> | 
| <p>JET_errTaskDropped<br />-106</p> | <p>Не удалось выполнить запрошенную асинхронную задачу.</p> | 
| <p>JET_errInternalError<br />-107</p> | <p>Произошла неустранимая внутренняя ошибка.</p> | 
| <p>JET_errDatabaseBufferDependenciesCorrupted<br />— 255</p> | <p>Неправильно заданы зависимости буфера, и произошла ошибка восстановления.</p> | 
| <p>JET_errPreviousVersion<br />— 322</p> | <p>Версия уже существовала, и произошла ошибка восстановления. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errPageBoundary<br />— 323</p> | <p>Достигнута граница страницы. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errKeyBoundary<br />— 324</p> | <p>Достигнута граница ключа. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errBadPageLink<br />— 327</p> | <p>База данных повреждена. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errBadBookmark<br />— 328</p> | <p>Закладка не имеет соответствующего адреса в базе данных. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errNTSystemCallFailed<br />— 334</p> | <p>Сбой вызова операционной системы. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errBadParentPageLink<br />— 338</p> | <p>Родительская база данных повреждена. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errSPAvailExtCacheOutOfSync<br />— 340</p> | <p>Кэш Аваилекст не соответствует дереву B +. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errSPAvailExtCorrupted<br />— 341</p> | <p>Дерево пространства Аллаваилекст повреждено. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errSPAvailExtCacheOutOfMemory<br />— 342</p> | <p>Произошла ошибка нехватки памяти при выделении узла кэша Аваилекст. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errSPOwnExtCorrupted<br />— 343</p> | <p>Дерево пространства Овнекст повреждено. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errDbTimeCorrupted<br />— 344</p> | <p>Дбтиме на текущей странице больше, чем глобальная база данных дбтиме. Эта ошибка возвращается диспетчером каталогов.</p> | 
| <p>JET_errKeyTruncated<br />— 346</p> | <p>Попытка создать ключ для элемента индекса завершилась неудачей, так как ключ был усечен, а определение индекса не разрешает усечение ключа.</p> | 
| <p>JET_errKeyTooBig<br />— 408</p> | <p>Слишком большой ключ. Эта ошибка возвращается диспетчером записей.</p> | 
| <p>JET_errInvalidLoggedOperation<br />-500</p> | <p>Не удается выполнить запротоколированную операцию.</p> | 
| <p>JET_errLogFileCorrupt<br />— 501</p> | <p>Файл журнала поврежден.</p> | 
| <p>JET_errNoBackupDirectory<br />— 503</p> | <p>Не указан каталог резервного копирования.</p> | 
| <p>JET_errBackupDirectoryNotEmpty<br />— 504</p> | <p>Каталог резервного копирования не пуст.</p> | 
| <p>JET_errBackupInProgress<br />— 505</p> | <p>Резервная копия уже активна.</p> | 
| <p>JET_errRestoreInProgress<br />— 506</p> | <p>Выполняется восстановление.</p> | 
| <p>JET_errMissingPreviousLogFile<br />— 509</p> | <p>Отсутствует файл журнала для контрольной точки.</p> | 
| <p>JET_errLogWriteFail<br />— 510</p> | <p>Ошибка записи в файл журнала.</p> | 
| <p>JET_errLogDisabledDueToRecoveryFailure<br />— 511</p> | <p>Попытка записи в журнал после сбоя восстановления.</p> | 
| <p>JET_errCannotLogDuringRecoveryRedo<br />— 512</p> | <p>Попытка записи в журнал во время повтора восстановления завершилась сбоем.</p> | 
| <p>JET_errLogGenerationMismatch<br />— 513</p> | <p>Имя файла журнала не соответствует номеру внутреннего поколения.</p> | 
| <p>JET_errBadLogVersion<br />— 514</p> | <p>Версия файла журнала несовместима с версией ESE.</p> | 
| <p>JET_errInvalidLogSequence<br />— 515</p> | <p>Метка времени в следующем журнале не соответствует ожидаемой метке времени.</p> | 
| <p>JET_errLoggingDisabled<br />— 516</p> | <p>Журнал неактивен.</p> | 
| <p>JET_errLogBufferTooSmall<br />— 517</p> | <p>Буфер журнала слишком мал для восстановления.</p> | 
| <p>JET_errLogSequenceEnd<br />— 519</p> | <p>Превышен максимальный номер файла журнала.</p> | 
| <p>JET_errNoBackup<br />— 520</p> | <p>Резервное копирование не выполняется.</p> | 
| <p>JET_errInvalidBackupSequence<br />— 521</p> | <p>Вызов резервного копирования не является последовательным.</p> | 
| <p>JET_errBackupNotAllowedYet<br />— 523</p> | <p>В настоящее время невозможно выполнить резервное копирование.</p> | 
| <p>JET_errDeleteBackupFileFail<br />— 524</p> | <p>Не удалось удалить файл резервной копии.</p> | 
| <p>JET_errMakeBackupDirectoryFail<br />— 525</p> | <p>Не удалось создать временный каталог резервного копирования.</p> | 
| <p>JET_errInvalidBackup<br />— 526</p> | <p>Циклическое ведение журнала включено; невозможно выполнить добавочное резервное копирование.</p> | 
| <p>JET_errRecoveredWithErrors<br />— 527</p> | <p>Данные были восстановлены с ошибками.</p> | 
| <p>JET_errMissingLogFile<br />— 528</p> | <p>Текущий файл журнала отсутствует.</p> | 
| <p>JET_errLogDiskFull<br />— 529</p> | <p>Диск журнала заполнен.</p> | 
| <p>JET_errBadLogSignature<br />— 530</p> | <p>Неверная подпись для файла журнала.</p> | 
| <p>JET_errBadDbSignature<br />— 531</p> | <p>Неверная подпись для файла базы данных.</p> | 
| <p>JET_errBadCheckpointSignature<br />— 532</p> | <p>Неверное описание файла контрольных точек.</p> | 
| <p>JET_errCheckpointCorrupt<br />— 533</p> | <p>Файл контрольных точек не найден или поврежден.</p> | 
| <p>JET_errMissingPatchPage<br />— 534</p> | <p>Страница файла исправления базы данных не найдена во время восстановления.</p> | 
| <p>JET_errBadPatchPage<br />— 535</p> | <p>Недопустимая страница файла исправления базы данных.</p> | 
| <p>JET_errRedoAbruptEnded<br />— 536</p> | <p>Непредвиденное завершение операции повтора из-за внезапного сбоя при чтении журналов из файла журнала.</p> | 
| <p>JET_errBadSLVSignature<br />— 537</p> | <p>Этот флаг зарезервирован.</p> | 
| <p>JET_errPatchFileMissing<br />— 538</p> | <p>При сложном восстановлении обнаружено, что в резервном наборе данных отсутствует файл исправления.</p> | 
| <p>JET_errDatabaseLogSetMismatch<br />— 539</p> | <p>База данных не принадлежит текущему набору файлов журнала.</p> | 
| <p>JET_errDatabaseStreamingFileMismatch<br />— 540</p> | <p>Этот флаг зарезервирован.</p> | 
| <p>JET_errLogFileSizeMismatch<br />— 541</p> | <p>Фактический размер файла журнала не совпадает с <a href="gg269235(v=exchg.10).md">JET_paramLogFileSize</a>.</p> | 
| <p>JET_errCheckpointFileNotFound<br />— 542</p> | <p>Не удалось найти файл контрольных точек.</p> | 
| <p>JET_errRequiredLogFilesMissing<br />— 543</p> | <p>Отсутствуют необходимые файлы журнала для восстановления.</p> | 
| <p>JET_errSoftRecoveryOnBackupDatabase<br />— 544</p> | <p>Мягкое восстановление будет использоваться в базе данных резервного копирования, когда вместо этого следует использовать восстановление.</p> | 
| <p>JET_errLogFileSizeMismatchDatabasesConsistent<br />— 545</p> | <p>Базы данных восстановлены, но размер файла журнала, используемый во время восстановления, не соответствует <a href="gg269235(v=exchg.10).md">JET_paramLogFileSize</a>.</p> | 
| <p>JET_errLogSectorSizeMismatch<br />— 546</p> | <p>Размер сектора файла журнала не совпадает с размером сектора текущего тома.</p> | 
| <p>JET_errLogSectorSizeMismatchDatabasesConsistent<br />— 547</p> | <p>Базы данных восстановлены, но размер сектора файла журнала (используемый во время восстановления) не совпадает с размером сектора текущего тома.</p> | 
| <p>JET_errLogSequenceEndDatabasesConsistent<br />— 548</p> | <p>Базы данных восстановлены, но использовались все возможные поколения журналов в текущей последовательности. Перед продолжением необходимо удалить все файлы журналов и файл контрольных точек, а также создать резервные копии баз данных.</p> | 
| <p>JET_errStreamingDataNotLogged<br />— 549</p> | <p>Недопустимая попытка воспроизвести операцию потокового файла, в которой данные не были занесены в журнал. Возможно, это вызвано попыткой Накату с включением циклического ведения журнала.</p> | 
| <p>JET_errDatabaseDirtyShutdown<br />— 550</p> | <p>Работа базы данных не была завершена аккуратно. Сначала необходимо выполнить восстановление, чтобы правильно завершить операции с базой данных для предыдущего завершения работы.</p> | 
| <p>JET_errDatabaseInconsistent<br />JET_errDatabaseDirtyShutdown</p> | <p>Эта ошибка устарела и была заменена JET_errDatabaseDirtyShutdown.</p> | 
| <p>JET_errConsistentTimeMismatch<br />— 551</p> | <p>Последнее согласованное время для базы данных не сопоставлено.</p> | 
| <p>JET_errDatabasePatchFileMismatch<br />— 552</p> | <p>Файл исправления базы данных не создается из этой резервной копии.</p> | 
| <p>JET_errEndingRestoreLogTooLow<br />— 553</p> | <p>Начальный номер журнала слишком мал для восстановления.</p> | 
| <p>JET_errStartingRestoreLogTooHigh<br />— 554</p> | <p>Начальный номер журнала слишком велик для восстановления.</p> | 
| <p>JET_errGivenLogFileHasBadSignature<br />— 555</p> | <p>Файл журнала восстановления имеет неправильную подпись.</p> | 
| <p>JET_errGivenLogFileIsNotContiguous<br />— 556</p> | <p>Файл журнала восстановления не является смежным.</p> | 
| <p>JET_errMissingRestoreLogFiles<br />— 557</p> | <p>Отсутствуют некоторые файлы журнала восстановления.</p> | 
| <p>JET_errMissingFullBackup<br />— 560</p> | <p>Перед попыткой выполнить добавочное резервное копирование база данных пропустила предыдущую полную резервную копию.</p> | 
| <p>JET_errBadBackupDatabaseSize<br />— 561</p> | <p>Размер базы данных резервного копирования не кратен размеру страницы базы данных.</p> | 
| <p>JET_errDatabaseAlreadyUpgraded<br />— 562</p> | <p>Текущая попытка обновить базу данных остановлена, так как база данных уже является текущей.</p> | 
| <p>JET_errDatabaseIncompleteUpgrade<br />— 563</p> | <p>База данных была частично преобразована в текущий формат. База данных должна быть восстановлена из резервной копии.</p> | 
| <p>JET_errMissingCurrentLogFiles<br />— 565</p> | <p>Некоторые текущие файлы журнала отсутствуют для непрерывного восстановления.</p> | 
| <p>JET_errDbTimeTooOld<br />— 566</p> | <p>Дбтиме на странице меньше, чем Дбтимебефоре в записи.</p> | 
| <p>JET_errDbTimeTooNew<br />— 567</p> | <p>Дбтиме на странице предварительно находится в Дбтимебефоре, который находится в записи.</p> | 
| <p>JET_errMissingFileToBackup<br />— 569</p> | <p>Некоторые файлы журнала или исправления базы данных отсутствовали во время резервного копирования.</p> | 
| <p>JET_errLogTornWriteDuringHardRestore<br />— 570</p> | <p>В резервной копии, заданной во время жесткого восстановления, обнаружена разорванная запись.</p> | 
| <p>JET_errLogTornWriteDuringHardRecovery<br />— 571</p> | <p>Обнаружена разорванная запись во время жесткого восстановления (журнал не был частью резервного набора данных).</p> | 
| <p>JET_errLogCorruptDuringHardRestore<br />— 573</p> | <p>Во время жесткого восстановления обнаружено повреждение в резервном наборе данных.</p> | 
| <p>JET_errLogCorruptDuringHardRecovery<br />— 574</p> | <p>Во время жесткого восстановления обнаружено повреждение (журнал не был частью резервного набора данных).</p> | 
| <p>JET_errMustDisableLoggingForDbUpgrade<br />— 575</p> | <p>Ведение журнала невозможно включить при попытке обновления базы данных.</p> | 
| <p>JET_errBadRestoreTargetInstance<br />— 577</p> | <p>Либо TargetInstance, который был указан для восстановления, не найден, либо файлы журнала не совпадают.</p> | 
| <p>JET_errRecoveredWithoutUndo<br />— 579</p> | <p>Ядро СУБД успешно воспроизводило все операции в журнале транзакций, чтобы выполнить восстановление после сбоя, но вызывающий объект, выбранный для отмены восстановления без отката незафиксированных обновлений.</p> | 
| <p>JET_errDatabasesNotFromSameSnapshot<br />— 580</p> | <p>Восстанавливаемые базы данных не относятся к одной резервной копии теневого копирования.</p> | 
| <p>JET_errSoftRecoveryOnSnapshot<br />— 581</p> | <p>Существует мягкое восстановление базы данных из резервного набора данных теневого копирования.</p> | 
| <p>JET_errUnicodeTranslationBufferTooSmall<br />— 601</p> | <p>Буфер преобразования Юникода слишком мал.</p> | 
| <p>JET_errUnicodeTranslationFail<br />— 602</p> | <p>Сбой нормализации Юникода.</p> | 
| <p>JET_errUnicodeNormalizationNotSupported<br />— 603</p> | <p>Операционная система не поддерживает нормализацию Юникода, и обратный вызов нормализации не был указан.</p> | 
| <p>JET_errExistingLogFileHasBadSignature<br />— 610</p> | <p>Существующий файл журнала имеет неправильную подпись.</p> | 
| <p>JET_errExistingLogFileIsNotContiguous<br />— 611</p> | <p>Существующий файл журнала не является смежным.</p> | 
| <p>JET_errLogReadVerifyFailure<br />— 612</p> | <p>В файле журнала во время резервного копирования обнаружена ошибка контрольной суммы.</p> | 
| <p>JET_errSLVReadVerifyFailure<br />— 613</p> | <p>Этот флаг зарезервирован.</p> | 
| <p>JET_errCheckpointDepthTooDeep<br />— 614</p> | <p>Существует слишком много невыполненных поколений между контрольной точкой и текущим поколением.</p> | 
| <p>JET_errRestoreOfNonBackupDatabase<br />— 615</p> | <p>Предпринята попытка принудительного восстановления базы данных, которая не является резервной базой данных.</p> | 
| <p>JET_errInvalidGrbit<br />— 900</p> | <p>Недопустимый параметр грбит.</p> | 
| <p>JET_errTermInProgress<br />–1000</p> | <p>Выполняется завершение.</p> | 
| <p>JET_errFeatureNotAvailable<br />— 1001</p> | <p>Этот элемент API не поддерживается.</p> | 
| <p>JET_errInvalidName<br />— 1002</p> | <p>Используется недопустимое имя.</p> | 
| <p>JET_errInvalidParameter<br />— 1003</p> | <p>Используется недопустимый параметр API.</p> | 
| <p>JET_errDatabaseFileReadOnly<br />— 1008</p> | <p>Попытка присоединиться к файлу базы данных, доступному только для чтения, для операций чтения и записи.</p> | 
| <p>JET_errInvalidDatabaseId<br />— 1010</p> | <p>Недопустимый идентификатор базы данных.</p> | 
| <p>JET_errOutOfMemory<br />— 1011</p> | <p>Системе не хватает памяти.</p> | 
| <p>JET_errOutOfDatabaseSpace<br />— 1012</p> | <p>Достигнут максимальный размер базы данных.</p> | 
| <p>JET_errOutOfCursors<br />— 1013</p> | <p>Таблица находится за пределами курсоров.</p> | 
| <p>JET_errOutOfBuffers<br />— 1014</p> | <p>В базе данных недостаточно буферов страниц.</p> | 
| <p>JET_errTooManyIndexes<br />— 1015</p> | <p>Слишком много индексов.</p> | 
| <p>JET_errTooManyKeys<br />— 1016</p> | <p>Слишком много столбцов в индексе.</p> | 
| <p>JET_errRecordDeleted<br />— 1017</p> | <p>Запись была удалена.</p> | 
| <p>JET_errReadVerifyFailure<br />— 1018</p> | <p>Ошибка контрольной суммы на странице базы данных.</p> | 
| <p>JET_errPageNotInitialized<br />— 1019</p> | <p>Пустая страница базы данных.</p> | 
| <p>JET_errOutOfFileHandles<br />— 1020</p> | <p>Дескрипторы файлов отсутствуют.</p> | 
| <p>JET_errDiskIO<br />— 1022</p> | <p>Ошибка ввода-вывода на диск.</p> | 
| <p>JET_errInvalidPath<br />— 1023</p> | <p>Недопустимый путь к файлу.</p> | 
| <p>JET_errInvalidSystemPath<br />— 1024</p> | <p>Недопустимый системный путь.</p> | 
| <p>JET_errInvalidLogDirectory<br />— 1025</p> | <p>Недопустимый каталог журнала.</p> | 
| <p>JET_errRecordTooBig<br />— 1026</p> | <p>Запись больше, чем максимальный размер.</p> | 
| <p>JET_errTooManyOpenDatabases<br />— 1027</p> | <p>Слишком много открытых баз данных.</p> | 
| <p>JET_errInvalidDatabase<br />— 1028</p> | <p>Это не файл базы данных.</p> | 
| <p>JET_errNotInitialized<br />— 1029</p> | <p>Ядро СУБД не инициализировано.</p> | 
| <p>JET_errAlreadyInitialized<br />— 1030</p> | <p>Ядро СУБД уже инициализировано.</p> | 
| <p>JET_errInitInProgress<br />— 1031</p> | <p>Инициализируется ядро СУБД.</p> | 
| <p>JET_errFileAccessDenied<br />— 1032</p> | <p>Не удается получить доступ к файлу, так как файл заблокирован или используется.</p> | 
| <p>JET_errBufferTooSmall<br />— 1038</p> | <p>Буфер слишком мал.</p> | 
| <p>JET_errTooManyColumns<br />— 1040</p> | <p>Определено слишком много столбцов.</p> | 
| <p>JET_errContainerNotEmpty<br />— 1043</p> | <p>Контейнер не пуст.</p> | 
| <p>JET_errInvalidFilename<br />— 1044</p> | <p>Недопустимое имя файла.</p> | 
| <p>JET_errInvalidBookmark<br />— 1045</p> | <p>Недопустимая закладка.</p> | 
| <p>JET_errColumnInUse<br />— 1046</p> | <p>Используемый столбец находится в индексе.</p> | 
| <p>JET_errInvalidBufferSize<br />— 1047</p> | <p>Буфер данных не соответствует размеру столбца.</p> | 
| <p>JET_errColumnNotUpdatable<br />— 1048</p> | <p>Не удается задать значение столбца.</p> | 
| <p>JET_errIndexInUse<br />— 1051</p> | <p>Индекс используется.</p> | 
| <p>JET_errLinkNotSupported<br />— 1052</p> | <p>Ссылка недоступна.</p> | 
| <p>JET_errNullKeyDisallowed<br />— 1053</p> | <p>Ключи NULL не допускаются в индексе.</p> | 
| <p>JET_errNotInTransaction<br />— 1054</p> | <p>Операция должна выполняться в рамках транзакции.</p> | 
| <p>JET_errTooManyActiveUsers<br />— 1059</p> | <p>Слишком много активных пользователей базы данных</p> | 
| <p>JET_errInvalidCountry<br />— 1061</p> | <p>Недопустимый или неизвестный код страны.</p> | 
| <p>JET_errInvalidLanguageId<br />— 1062</p> | <p>Недопустимый или Неизвестный идентификатор языка.</p> | 
| <p>JET_errInvalidCodePage<br />— 1063</p> | <p>Недопустимая или неизвестная кодовая страница.</p> | 
| <p>JET_errInvalidLCMapStringFlags<br />— 1064</p> | <p>Для <a href="/windows/win32/api/winnls/nf-winnls-lcmapstringa">LCMapString завершилось ошибкой</a>используются недопустимые флаги.</p> | 
| <p>JET_errVersionStoreEntryTooBig<br />— 1065</p> | <p>Попытка создать запись в хранилище версий (RCE), которая была больше, чем у контейнера версий.</p> | 
| <p>JET_errVersionStoreOutOfMemoryAndCleanupTimedOut<br />— 1066</p> | <p>В хранилище версий недостаточно памяти, попытка очистки завершилась сбоем.</p> | 
| <p>JET_errVersionStoreOutOfMemory<br />— 1069</p> | <p>В хранилище версий недостаточно памяти, и уже была предпринята попытка очистки.</p> | 
| <p>JET_errCannotIndex<br />— 1071</p> | <p>Столбцы депонирования и SLV не могут быть проиндексированы.</p> | 
| <p>JET_errRecordNotDeleted<br />— 1072</p> | <p>Запись не была удалена.</p> | 
| <p>JET_errTooManyMempoolEntries<br />— 1073</p> | <p>Запрошено слишком много записей мемпул.</p> | 
| <p>JET_errOutOfObjectIDs<br />— 1074</p> | <p>База данных находится за пределами объектов ObjectID дерева B +, поэтому для освобождения или неиспользуемых идентификаторов ObjectId необходимо выполнить автономную дефрагментацию.</p> | 
| <p>JET_errOutOfLongValueIDs<br />— 1075</p> | <p>Счетчик с ИДЕНТИФИКАТОРом длинных значений достиг максимального значения. Для освобождения бесплатной или неиспользуемой Лонгвалуеидс необходимо выполнить автономную дефрагментацию.</p> | 
| <p>JET_errOutOfAutoincrementValues<br />— 1076</p> | <p>Счетчик автоматического приращения достиг максимального значения. Автономная дефрагментация не сможет освободить свободные или неиспользуемые значения автоинкремента.</p> | 
| <p>JET_errOutOfDbtimeValues<br />— 1077</p> | <p>Счетчик Дбтиме достиг максимального значения. Для освобождения бесплатных или неиспользуемых значений Дбтиме необходимо выполнить автономную дефрагментацию.</p> | 
| <p>JET_errOutOfSequentialIndexValues<br />— 1078</p> | <p>Достигнуто максимальное значение счетчика последовательных индексов. Для освобождения бесплатных или неиспользуемых значений Секуентиалиндекс необходимо выполнить автономную дефрагментацию.</p> | 
| <p>JET_errRunningInOneInstanceMode<br />— 1080</p> | <p>В этом вызове с несколькими экземплярами включен режим с одним экземпляром.</p> | 
| <p>JET_errRunningInMultiInstanceMode<br />— 1081</p> | <p>В этом вызове одного экземпляра включен режим с несколькими экземплярами.</p> | 
| <p>JET_errSystemParamsAlreadySet<br />— 1082</p> | <p>Глобальные системные параметры уже заданы.</p> | 
| <p>JET_errSystemPathInUse<br />— 1083</p> | <p>Системный путь уже используется другим экземпляром базы данных.</p> | 
| <p>JET_errLogFilePathInUse<br />— 1084</p> | <p>Путь к файлу журнала уже используется другим экземпляром базы данных.</p> | 
| <p>JET_errTempPathInUse<br />— 1085</p> | <p>Путь к временной базе данных уже используется другим экземпляром базы данных.</p> | 
| <p>JET_errInstanceNameInUse<br />— 1086</p> | <p>Имя экземпляра уже используется.</p> | 
| <p>JET_errInstanceUnavailable<br />— 1090</p> | <p>Этот экземпляр нельзя использовать, так как в нем возникла неустранимая ошибка.</p> | 
| <p>JET_errDatabaseUnavailable<br />— 1091</p> | <p>Эту базу данных невозможно использовать, так как произошла неустранимая ошибка.</p> | 
| <p>JET_errInstanceUnavailableDueToFatalLogDiskFull<br />— 1092</p> | <p>Этот экземпляр не может быть использован, так как при выполнении операции (например, откат транзакции), которая не допускает ошибок, произошла ошибка переполнения журнала диска.</p> | 
| <p>JET_errOutOfSessions<br />— 1101</p> | <p>В базе данных недостаточно сеансов.</p> | 
| <p>JET_errWriteConflict<br />— 1102</p> | <p>Сбой блокировки записи из-за существования ожидающей блокировки записи.</p> | 
| <p>JET_errTransTooDeep<br />— 1103</p> | <p>Слишком глубокая вложенность транзакций.</p> | 
| <p>JET_errInvalidSesid<br />— 1104</p> | <p>Недопустимый обработчик сеанса.</p> | 
| <p>JET_errWriteConflictPrimaryIndex<br />— 1105</p> | <p>Попытка обновления для незафиксированного первичного индекса.</p> | 
| <p>JET_errInTransaction<br />— 1108</p> | <p>Операция не разрешена в рамках транзакции.</p> | 
| <p>JET_errRollbackRequired<br />— 1109</p> | <p>Должна быть произведена откат текущей транзакции. Она не может быть зафиксирована, и не может быть запущена новая.</p> | 
| <p>JET_errTransReadOnly<br />— 1110</p> | <p>Транзакция, доступная только для чтения, попыталась изменить базу данных.</p> | 
| <p>JET_errSessionWriteConflict<br />— 1111</p> | <p>Предпринята попытка заменить одну и ту же запись двумя разными курсорами в одном сеансе.</p> | 
| <p>JET_errRecordTooBigForBackwardCompatibility<br />— 1112</p> | <p>Запись будет слишком большой, если она представлена в формате базы данных из предыдущей версии Jet.</p> | 
| <p>JET_errCannotMaterializeForwardOnlySort<br />— 1113</p> | <p>Не удалось создать временную таблицу из-за параметров, конфликтующих с JET_bitTTForwardOnly.</p> | 
| <p>JET_errSesidTableIdMismatch<br />— 1114</p> | <p>Невозможно использовать этот обработчик сеанса с идентификатором таблицы, так как он не использовался для его создания.</p> | 
| <p>JET_errInvalidInstance<br />— 1115</p> | <p>Недопустимый указатель экземпляра или ссылка на экземпляр, который был закрыт.</p> | 
| <p>JET_errReadLostFlushVerifyFailure<br />— 1119</p> | <p>На странице базы данных, считанной с диска, была записана Предыдущая запись, не представленная на странице. доступно в Windows 8 и более поздних версиях для клиента, а Windows Server 2012 и более поздних версий для сервера.</p> | 
| <p>JET_errDatabaseDuplicate<br />— 1201</p> | <p>База данных уже существует.</p> | 
| <p>JET_errDatabaseInUse<br />— 1202</p> | <p>Используемая база данных.</p> | 
| <p>JET_errDatabaseNotFound<br />— 1203</p> | <p>Такая база данных отсутствует.</p> | 
| <p>JET_errDatabaseInvalidName<br />— 1204</p> | <p>Недопустимое имя базы данных.</p> | 
| <p>JET_errDatabaseInvalidPages<br />— 1205</p> | <p>Недопустимое число страниц.</p> | 
| <p>JET_errDatabaseCorrupted<br />— 1206</p> | <p>Отсутствует файл, отличный от базы данных, или повреждена база данных.</p> | 
| <p>JET_errDatabaseLocked<br />— 1207</p> | <p>База данных заблокирована в монопольном режиме.</p> | 
| <p>JET_errCannotDisableVersioning<br />— 1208</p> | <p>Не удается отключить управление версиями для этой базы данных.</p> | 
| <p>JET_errInvalidDatabaseVersion<br />— 1209</p> | <p>Ядро СУБД несовместимо с базой данных.</p> | 
| <p>JET_errDatabase200Format<br />— 1210</p> | <p>База данных имеет более старый формат (200). Эта ошибка возвращается функцией <a href="gg294068(v=exchg.10).md">жетинит</a> , если задан параметр <a href="gg269337(v=exchg.10).md">JET_paramCheckFormatWhenOpenFail</a> . только Windows NT клиент.</p> | 
| <p>JET_errDatabase400Format<br />— 1211</p> | <p>База данных имеет более старый формат (400). Эта ошибка возвращается функцией <a href="gg294068(v=exchg.10).md">жетинит</a> , если задан параметр <a href="gg269337(v=exchg.10).md">JET_paramCheckFormatWhenOpenFail</a> . только Windows NT клиент.</p> | 
| <p>JET_errDatabase500Format<br />— 1212</p> | <p>База данных имеет более старый формат (500). Эта ошибка возвращается функцией <a href="gg294068(v=exchg.10).md">жетинит</a> , если задан параметр <a href="gg269337(v=exchg.10).md">JET_paramCheckFormatWhenOpenFail</a> . только Windows NT клиент.</p> | 
| <p>JET_errPageSizeMismatch<br />— 1213</p> | <p>Размер страницы базы данных не соответствует подсистеме.</p> | 
| <p>JET_errTooManyInstances<br />— 1214</p> | <p>Больше нельзя запускать экземпляры базы данных.</p> | 
| <p>JET_errDatabaseSharingViolation<br />— 1215</p> | <p>База данных используется другим экземпляром базы данных.</p> | 
| <p>JET_errAttachedDatabaseMismatch<br />— 1216</p> | <p>Необработанное вложение базы данных обнаружено в начале или в конце восстановления, но база данных отсутствует или не соответствует сведениям о вложении.</p> | 
| <p>JET_errDatabaseInvalidPath<br />— 1217</p> | <p>Указан недопустимый путь к файлу базы данных.</p> | 
| <p>JET_errDatabaseIdInUse<br />— 1218</p> | <p>Базе данных назначается идентификатор, который уже используется.</p> | 
| <p>JET_errForceDetachNotAllowed<br />— 1219</p> | <p>Принудительная отсоединение разрешена только после того, как нормальная отсоединение была остановлена из-за ошибки.</p> | 
| <p>JET_errCatalogCorrupted<br />— 1220</p> | <p>В каталоге обнаружено повреждение.</p> | 
| <p>JET_errPartiallyAttachedDB<br />— 1221</p> | <p>База данных присоединена только частично, а операция присоединения не может быть завершена.</p> | 
| <p>JET_errDatabaseSignInUse<br />— 1222</p> | <p>База данных с такой же подписью уже используется.</p> | 
| <p>JET_errDatabaseCorruptedNoRepair<br />— 1224</p> | <p>База данных повреждена, но восстановление не разрешено.</p> | 
| <p>JET_errInvalidCreateDbVersion<br />— 1225</p> | <p>Ядро СУБД попыталось воспроизвести операцию создания базы данных из журнала транзакций, но не удалось выполнить из-за несовместимой версии этой операции.</p> | 
| <p>JET_errTableLocked<br />— 1302</p> | <p>Таблица монопольно заблокирована.</p> | 
| <p>JET_errTableDuplicate<br />— 1303</p> | <p>Таблица уже существует.</p> | 
| <p>JET_errTableInUse<br />— 1304</p> | <p>Таблица используется и не может быть заблокирована.</p> | 
| <p>JET_errObjectNotFound<br />— 1305</p> | <p>Такой таблицы или объекта нет.</p> | 
| <p>JET_errDensityInvalid<br />— 1307</p> | <p>Недопустимая плотность файла или индекса.</p> | 
| <p>JET_errTableNotEmpty<br />— 1308</p> | <p>Таблица не пуста.</p> | 
| <p>JET_errInvalidTableId<br />— 1310</p> | <p>Недопустимый идентификатор таблицы.</p> | 
| <p>JET_errTooManyOpenTables<br />— 1311</p> | <p>Невозможно открыть больше таблиц даже после выполнения внутренней задачи очистки.</p> | 
| <p>JET_errIllegalOperation<br />— 1312</p> | <p>Операция не поддерживается для таблицы.</p> | 
| <p>JET_errTooManyOpenTablesAndCleanupTimedOut<br />— 1313</p> | <p>Не удается открыть больше таблиц, так как не удалось завершить попытку очистки.</p> | 
| <p>JET_errObjectDuplicate<br />— 1314</p> | <p>Имя таблицы или объекта используется.</p> | 
| <p>JET_errInvalidObject<br />— 1316</p> | <p>Объект недопустим для операции.</p> | 
| <p>JET_errCannotDeleteTempTable<br />— 1317</p> | <p>Для удаления временной таблицы необходимо использовать <a href="gg294087(v=exchg.10).md">жетклосетабле</a> вместо <a href="gg294128(v=exchg.10).md">жетделететабле</a> .</p> | 
| <p>JET_errCannotDeleteSystemTable<br />— 1318</p> | <p>Недопустимая попытка удалить системную таблицу.</p> | 
| <p>JET_errCannotDeleteTemplateTable<br />— 1319</p> | <p>Недопустимая попытка удалить таблицу шаблонов.</p> | 
| <p>JET_errExclusiveTableLockRequired<br />— 1322</p> | <p>Должна быть монопольная блокировка таблицы.</p> | 
| <p>JET_errFixedDDL<br />— 1323</p> | <p>В этой таблице запрещены операции DDL.</p> | 
| <p>JET_errFixedInheritedDDL<br />— 1324</p> | <p>В производной таблице операции DDL запрещены в наследуемой части DDL.</p> | 
| <p>JET_errCannotNestDDL<br />— 1325</p> | <p>Вложенные иерархические DDL в настоящее время не поддерживаются.</p> | 
| <p>JET_errDDLNotInheritable<br />— 1326</p> | <p>Предпринята попытка наследования DDL из таблицы, которая не помечена как таблица шаблона.</p> | 
| <p>JET_errInvalidSettings<br />— 1328</p> | <p>Системные параметры заданы неправильно.</p> | 
| <p>JET_errClientRequestToStopJetService<br />— 1329</p> | <p>Клиент запросил остановку службы.</p> | 
| <p>JET_errCannotAddFixedVarColumnToDerivedTable<br />— 1330</p> | <p>Таблица шаблона была создана с установленным флагом Нофикседварколумнсиндериведтаблес.</p> | 
| <p>JET_errIndexCantBuild<br />— 1401</p> | <p>Не удалось выполнить сборку индекса.</p> | 
| <p>JET_errIndexHasPrimary<br />— 1402</p> | <p>Первичный индекс уже определен.</p> | 
| <p>JET_errIndexDuplicate<br />— 1403</p> | <p>Индекс уже определен.</p> | 
| <p>JET_errIndexNotFound<br />— 1404</p> | <p>Такого индекса нет.</p> | 
| <p>JET_errIndexMustStay<br />— 1405</p> | <p>Невозможно удалить кластеризованный индекс.</p> | 
| <p>JET_errIndexInvalidDef<br />— 1406</p> | <p>Недопустимое определение индекса.</p> | 
| <p>JET_errInvalidCreateIndex<br />— 1409</p> | <p>Недопустимое создание описания индекса.</p> | 
| <p>JET_errTooManyOpenIndexes<br />— 1410</p> | <p>База данных выходит за пределы блоков описания индекса.</p> | 
| <p>JET_errMultiValuedIndexViolation<br />— 1411</p> | <p>Для многозначного индекса были созданы неуникальные ключи индексов между записями.</p> | 
| <p>JET_errIndexBuildCorrupted<br />— 1412</p> | <p>Вторичный индекс, который правильно отражает первичный индекс, не удалось построить.</p> | 
| <p>JET_errPrimaryIndexCorrupted<br />— 1413</p> | <p>Первичный индекс поврежден, и база данных должна быть дефрагментирована.</p> | 
| <p>JET_errSecondaryIndexCorrupted<br />— 1414</p> | <p>Вторичный индекс поврежден, и база данных должна быть дефрагментирована.</p> | 
| <p>JET_errInvalidIndexId<br />— 1416</p> | <p>Недопустимый идентификатор индекса.</p> | 
| <p>JET_errIndexTuplesSecondaryIndexOnly<br />— 1430</p> | <p>Индекс кортежа можно задать только для вторичного индекса.</p> | 
| <p>JET_errIndexTuplesTooManyColumns<br />— 1431</p> | <p>Определение индекса для индекса кортежа содержит дополнительные ключевые столбцы, которые может поддерживать ядро СУБД.</p><p><strong>Примечание  </strong> . JET_errIndexTuplesOneColumnOnlyная ошибка устарела и заменена JET_errIndexTuplesTooManyColumns.</p> | 
| <p>JET_errIndexTuplesNonUniqueOnly<br />— 1432</p> | <p>Индекс кортежа должен быть неуникальным индексом.</p> | 
| <p>JET_errIndexTuplesTextBinaryColumnsOnly<br />— 1433</p> | <p>Определение индекса кортежа может содержать только ключевые столбцы с типами столбцов text или binary.</p><p><strong>Примечание  </strong> . JET_errIndexTuplesTextColumnsOnlyная ошибка устарела и заменена JET_errIndexTuplesTextBinaryColumnsOnly.</p> | 
| <p>JET_errIndexTuplesVarSegMacNotAllowed<br />— 1434</p> | <p>Индекс кортежа не допускает настройки Кбварсегмак.</p> | 
| <p>JET_errIndexTuplesInvalidLimits<br />— 1435</p> | <p>Минимальная или максимальная длина кортежа или максимальное число символов, указанных для индекса, недопустимы.</p> | 
| <p>JET_errIndexTuplesCannotRetrieveFromIndex<br />— 1436</p> | <p><a href="gg269198(v=exchg.10).md">Жетретриевеколумн</a> не может быть вызван с установленным флагом JET_bitRetrieveFromIndex при извлечении столбца в индексе кортежа.</p> | 
| <p>JET_errIndexTuplesKeyTooSmall<br />— 1437</p> | <p>Указанный ключ не соответствует минимальной длине кортежа.</p> | 
| <p>JET_errColumnLong<br />— 1501</p> | <p>Значение столбца является длинным.</p> | 
| <p>JET_errColumnNoChunk<br />— 1502</p> | <p>Такой фрагмент не существует в длинном значении.</p> | 
| <p>JET_errColumnDoesNotFit<br />— 1503</p> | <p>Поле не будет помещаться в записи.</p> | 
| <p>JET_errNullInvalid<br />— 1504</p> | <p>Недопустимое значение null.</p> | 
| <p>JET_errColumnIllegalNull<br />JET_errNullInvalid</p> | <p>Недопустимое значение null. Эта ошибка возвращается диспетчером записей.</p> | 
| <p>JET_errColumnIndexed-1505</p> | <p>Столбец индексируется и не может быть удален.</p> | 
| <p>JET_errColumnTooBig-1506</p> | <p>Длина поля превышает максимально допустимую длину.</p> | 
| <p>JET_errColumnNotFound-1507</p> | <p>Такого столбца нет.</p> | 
| <p>JET_errColumnDuplicate-1508</p> | <p>Это поле уже определено.</p> | 
| <p>JET_errMultiValuedColumnMustBeTagged-1509</p> | <p>Предпринята попытка создать столбец с несколькими значениями, но столбец не был помечен.</p> | 
| <p>JET_errColumnRedundant-1510</p> | <p>Второй столбец с автоматическим приращением или версией.</p> | 
| <p>JET_errInvalidColumnType-1511</p> | <p>Недопустимый тип данных столбца.</p> | 
| <p>JET_errTaggedNotNULL-1514</p> | <p>Нет помеченных столбцов, относящихся к NULL.</p> | 
| <p>JET_errNoCurrentIndex-1515</p> | <p>База данных недопустима, так как она не содержит текущего индекса.</p> | 
| <p>JET_errKeyIsMade-1516</p> | <p>Ключ полностью создан.</p> | 
| <p>JET_errBadColumnId-1517</p> | <p>Неправильный идентификатор столбца.</p> | 
| <p>JET_errBadItagSequence-1518</p> | <p>Некорректный Итагсекуенце для столбца с тегами.</p> | 
| <p>JET_errColumnInRelationship-1519</p> | <p>Невозможно удалить столбец, так как он является частью связи.</p> | 
| <p>JET_errCannotBeTagged-1521</p> | <p>Автоматическое увеличение и версия не могут быть помечены.</p> | 
| <p>JET_errDefaultValueTooBig-1524</p> | <p>Значение по умолчанию превышает максимальный размер.</p> | 
| <p>JET_errMultiValuedDuplicate-1525</p> | <p>В уникальном столбце с несколькими значениями обнаружено повторяющееся значение.</p> | 
| <p>JET_errLVCorrupted-1526</p> | <p>Обнаружено повреждение в дереве длинных значений.</p> | 
| <p>JET_errMultiValuedDuplicateAfterTruncation-1528</p> | <p>Обнаружено повторяющееся значение в уникальном столбце с несколькими значениями после нормализации данных, и нормализация усекает данные перед сравнением.</p> | 
| <p>JET_errDerivedColumnCorruption-1529</p> | <p>Недопустимый столбец в производной таблице.</p> | 
| <p>JET_errInvalidPlaceholderColumn-1530</p> | <p>Предпринята попытка преобразовать столбец в заполнитель первичного индекса, но этот столбец не соответствует необходимым критериям.</p> | 
| <p>JET_errRecordNotFound-1601</p> | <p>Ключ не найден.</p> | 
| <p>JET_errRecordNoCopy-1602</p> | <p>Нет рабочего буфера.</p> | 
| <p>JET_errNoCurrentRecord-1603</p> | <p>Отсутствует текущая запись.</p> | 
| <p>JET_errRecordPrimaryChanged-1604</p> | <p>Первичный ключ может не измениться.</p> | 
| <p>JET_errKeyDuplicate-1605</p> | <p>Недопустимый дублирующийся ключ.</p> | 
| <p>JET_errAlreadyPrepared-1607</p> | <p>Предпринята попытка обновить запись, пока уже выполняется обновление записи.</p> | 
| <p>JET_errKeyNotMade-1608</p> | <p>Вызов не был сделан в <a href="gg269329(v=exchg.10).md">жетмакекэй</a>.</p> | 
| <p>JET_errUpdateNotPrepared-1609</p> | <p>Вызов не был сделан в <a href="gg269339(v=exchg.10).md">жетпрепареупдате</a>.</p> | 
| <p>JET_errDataHasChanged-1611</p> | <p>Данные были изменены, операция прервана.</p> | 
| <p>JET_errLanguageNotSupported-1619</p> | <p>эта Windowsная установка не поддерживает выбранный язык.</p> | 
| <p>JET_errTooManySorts-1701</p> | <p>Слишком много процессов сортировки.</p> | 
| <p>JET_errInvalidOnSort-1702</p> | <p>Во время сортировки произошла Недопустимая операция.</p> | 
| <p>JET_errTempFileOpenError-1803</p> | <p>Не удалось открыть временный файл.</p> | 
| <p>JET_errTooManyAttachedDatabases-1805</p> | <p>Открыто слишком много баз данных.</p> | 
| <p>JET_errDiskFull-1808</p> | <p>На диске не осталось места.</p> | 
| <p>JET_errPermissionDenied-1809</p> | <p>Отказано в разрешении.</p> | 
| <p>JET_errFileNotFound-1811</p> | <p>Файл не найден.</p> | 
| <p>JET_errFileInvalidType-1812</p> | <p>Недопустимый тип файла.</p> | 
| <p>JET_errAfterInitialization-1850</p> | <p>Невозможно запустить восстановление после инициализации.</p> | 
| <p>JET_errLogCorrupted-1852</p> | <p>Не удалось интерпретировать журналы.</p> | 
| <p>JET_errInvalidOperation-1906</p> | <p>Недопустимая операция.</p> | 
| <p>JET_errAccessDenied-1907</p> | <p>Отказано в доступе".</p> | 
| <p>JET_errTooManySplits-1909</p> | <p>Бесконечное разбиение.</p> | 
| <p>JET_errSessionSharingViolation-1910</p> | <p>Несколько потоков используют один сеанс.</p> | 
| <p>JET_errEntryPointNotFound-1911</p> | <p>Не удалось найти точку входа в требуемой библиотеке DLL.</p> | 
| <p>JET_errSessionContextAlreadySet-1912</p> | <p>Для указанного сеанса уже задан контекст сеанса.</p> | 
| <p>JET_errSessionContextNotSetByThisThread-1913</p> | <p>Предпринята попытка сбросить контекст сеанса, но текущий поток не был исходным, который задает контекст сеанса.</p> | 
| <p>JET_errSessionInUse-1914</p> | <p>Предпринята попытка завершить сеанс, который сейчас используется.</p> | 
| <p>JET_errRecordFormatConversionFailed-1915</p> | <p>Произошла внутренняя ошибка при преобразовании формата динамической записи.</p> | 
| <p>JET_errOneDatabasePerSession-1916</p> | <p>Допускается только одна открытая пользовательская база данных на сеанс (как указано установкой флага <a href="gg269337(v=exchg.10).md">JET_paramOneDatabasePerSession</a> во время создания базы данных).</p> | 
| <p>JET_errRollbackError-1917</p> | <p>Произошла ошибка во время отката.</p> | 
| <p>JET_errCallbackFailed-2101</p> | <p>Не удалось вызвать функцию обратного вызова.</p> | 
| <p>JET_errCallbackNotResolved-2102</p> | <p>Не удалось найти функцию обратного вызова.</p> | 
| <p>JET_errOSSnapshotInvalidSequence-2401</p> | <p>API теневого копирования операционной системы использован в недопустимой последовательности.</p> | 
| <p>JET_errOSSnapshotTimeOut-2402</p> | <p>Теневое копирование операционной системы завершилось с превышением времени ожидания.</p> | 
| <p>JET_errOSSnapshotNotAllowed-2403</p> | <p>Теневое копирование операционной системы запрещено, так как выполняется резервное копирование или восстановление.</p> | 
| <p>JET_errOSSnapshotInvalidSnapId-2404</p> | <p>Не удалось выполнить операцию, так как указан недопустимый маркер теневого копирования операционной системы.</p> | 
| <p>JET_errLSCallbackNotSpecified-3000</p> | <p>Предпринята попытка использовать локальное хранилище без указания функции обратного вызова.</p> | 
| <p>JET_errLSAlreadySet-3001</p> | <p>Была предпринята попытка задать локальное хранилище для объекта, который уже был задан.</p> | 
| <p>JET_errLSNotSet-3002</p> | <p>Предпринята попытка получить локальное хранилище из объекта, в котором он не был задан.</p> | 
| <p>JET_errFileIOSparse-4000</p> | <p>Не удалось выполнить операцию ввода-вывода, так как она была предпринята для нераспределенной области файла.</p> | 
| <p>JET_errFileIOBeyondEOF-4001</p> | <p>Операция чтения была выдана в расположение после конца файла (операции записи разворачивают файл).</p> | 
| <p>JET_errFileIOAbort-4002</p> | <p>Этот флаг указывает JET_ABORTRETRYFAILCALLBACK вызывающему объекту прервать указанный ввод-вывод.</p> | 
| <p>JET_errFileIORetry-4003</p> | <p>Этот флаг указывает JET_ABORTRETRYFAILCALLBACK вызывающему объекту повторить указанный ввод-вывод.</p> | 
| <p>JET_errFileIOFail-4004</p> | <p>Этот флаг указывает JET_ABORTRETRYFAILCALLBACK вызывающему объекту завершиться ошибкой указанного ввода-вывода.</p> | 
| <p>JET_errFileCompressed-4005</p> | <p>Доступ для чтения и записи не поддерживается для сжатых файлов.</p> | 



### <a name="remarks"></a>Комментарии

В общем случае значение, большее нуля, должно интерпретироваться как предупреждение, нулевое значение должно интерпретироваться как успешно, а значение меньше нуля должно интерпретироваться как ошибка. Никакие другие шаблоны в этих значениях, например диапазоны значений, должны быть полагаться на приложения.

### <a name="requirements"></a>Требования


| | | <p><strong>Клиент</strong></p> | <p>требуется Windows Vista, Windows XP или Windows 2000 Professional.</p> | | <p><strong>Сервер</strong></p> | <p>требуется Windows server 2008, Windows server 2003 или сервер Windows 2000.</p> | | <p><strong>Header</strong></p> | <p>Объявлено в ESENT. h.</p> | 



### <a name="see-also"></a>См. также:

[Параметры обработки ошибок](./error-handling-parameters.md)  
[ошибки расширенного обработчика служба хранилища](./extensible-storage-engine-errors.md)  
[расширяемые файлы служба хранилища Engine](./extensible-storage-engine-files.md)
