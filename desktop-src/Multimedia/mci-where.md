---
title: Команда MCI_WHERE (Ммсистем. h)
description: Команда MCI, \_ которая получает прямоугольник обрезки для видеоустройства.
ms.assetid: f64a7e49-4ee1-4836-ba9a-0bbdc47626b3
keywords:
- команда MCI_WHERE Windows мультимедиа
topic_type:
- apiref
api_name:
- MCI_WHERE
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
ms.openlocfilehash: f6619131319863d1159a3bdb8bb85d366243544a
ms.sourcegitcommit: 9eebab0ead09cecdbc24f5f84d56c8b6a7c22736
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/10/2021
ms.locfileid: "124369921"
---
# <a name="mci_where-command"></a>\_Команда MCI WHERE

Команда MCI, \_ которая получает прямоугольник обрезки для видеоустройства. Эта команда распознает цифровые видеоролики и устройства наложения видео. **Верхний** и **левый** элементы возвращенного [Rect](/previous-versions//ms536136(v=vs.85)) содержат источник прямоугольника обрезки, а **правый** и **Нижний** элементы содержат ширину и высоту прямоугольника обрезки. (Это не стандартное использование **правых** и **нижних** элементов.)

Чтобы отправить эту команду, вызовите функцию [**мЦисендкомманд**](/previous-versions//dd757160(v=vs.85)) со следующими параметрами.


```C++
MCIERROR mciSendCommand(
  MCIDEVICEID wDeviceID, 
  MCI_WHERE, 
  DWORD dwFlags, 
  (DWORD) (LPMCI_GENERIC_PARMS) lpQuery
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

<span id="wDeviceID"></span><span id="wdeviceid"></span><span id="WDEVICEID"></span>*вдевицеид*
</dt> <dd>

Идентификатор устройства MCI, который должен получить командное сообщение.

</dd> <dt>

<span id="dwFlags"></span><span id="dwflags"></span><span id="DWFLAGS"></span>*dwFlags*
</dt> <dd>

\_Уведомление MCI, \_ Ожидание MCI или, для устройств с цифровыми видео, \_ тест MCI. Дополнительные сведения об этих флагах см. [в разделе Флаги ожидания, уведомления и проверки](the-wait-notify-and-test-flags.md).

</dd> <dt>

<span id="lpQuery"></span><span id="lpquery"></span><span id="LPQUERY"></span>*лпкуери*
</dt> <dd>

Указатель на [**общую структуру \_ \_ пармс MCI**](mci-generic-parms.md) . (Устройства с расширенными наборами команд могут заменить эту структуру структурой, зависящей от устройства.)

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает нуль в случае успеха или ошибку в противном случае.

## <a name="remarks"></a>Remarks

С типом устройства **дигиталвидео** используются следующие дополнительные флаги:

<dl> <dt>

<span id="MCI_DGV_WHERE_DESTINATION"></span><span id="mci_dgv_where_destination"></span>MCI \_ ДГВ, \_ где \_ Destination
</dt> <dd>

Получает описание прямоугольной области, используемой для вывода видео и изображений в клиентской области текущего окна.

</dd> <dt>

<span id="MCI_DGV_WHERE_FRAME"></span><span id="mci_dgv_where_frame"></span>MCI \_ ДГВ, \_ где \_ Frame
</dt> <dd>

Получает описание прямоугольной области буфера кадров, в которой масштабируются изображения из прямоугольника видео. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> <dt>

<span id="MCI_DGV_WHERE_MAX"></span><span id="mci_dgv_where_max"></span>MCI \_ ДГВ, \_ где \_ Max
</dt> <dd>

При использовании с MCI \_ ДГВ \_ \_ , где Destination или \_ MCI \_ ДГВ \_ , где Source, возвращаемый прямоугольник указывает максимальную ширину и высоту указанной области. При использовании с MCI \_ ДГВ \_ \_ , где Window, возвращаемый прямоугольник указывает размер всего экрана.

</dd> <dt>

<span id="MCI_DGV_WHERE_SOURCE"></span><span id="mci_dgv_where_source"></span>MCI \_ ДГВ, \_ где \_ Source
</dt> <dd>

Получает описание прямоугольной области (обрезанной из буфера кадров), которая растягивается в соответствии с прямоугольником назначения на экране.

</dd> <dt>

<span id="MCI_DGV_WHERE_VIDEO"></span><span id="mci_dgv_where_video"></span>MCI \_ ДГВ, \_ где \_ видео
</dt> <dd>

Получает описание прямоугольной области, обрезанной от источника презентации, для заполнения прямоугольника фрейма в буфере кадров. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> <dt>

<span id="MCI_DGV_WHERE_WINDOW"></span><span id="mci_dgv_where_window"></span>MCI \_ ДГВ, \_ где \_ окно
</dt> <dd>

Получает описание рамки для окна просмотра.

</dd> <dt>


</dt> <dd></dd> </dl>

Для устройств с цифровыми видео параметр *лпкуери* указывает на **ДГВ MCI, где \_ Структура \_ \_ пармс** . **ДГВ MCI \_ , \_ где структура \_ Пармс** идентична структуре [**MCI \_ ДГВ \_ Rect \_ пармс**](/windows/win32/api/digitalv/ns-digitalv-mci_dgv_rect_parms) .

Для типа устройства **наложения** используются следующие дополнительные флаги:

<dl> <dt>

<span id="MCI_OVLY_WHERE_DESTINATION"></span><span id="mci_ovly_where_destination"></span>MCI \_ овли, \_ где \_ Destination
</dt> <dd>

Получает конечный прямоугольник для вывода. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> <dt>

<span id="MCI_OVLY_WHERE_FRAME"></span><span id="mci_ovly_where_frame"></span>MCI \_ овли, \_ где \_ Frame
</dt> <dd>

Получает прямоугольник наложенного фрейма. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> <dt>

<span id="MCI_OVLY_WHERE_SOURCE"></span><span id="mci_ovly_where_source"></span>MCI \_ овли, \_ где \_ Source
</dt> <dd>

Получает исходный прямоугольник. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> <dt>

<span id="MCI_OVLY_WHERE_VIDEO"></span><span id="mci_ovly_where_video"></span>MCI \_ овли, \_ где \_ видео
</dt> <dd>

Получает прямоугольник видео. Координаты прямоугольника помещаются в элемент **RC** структуры, идентифицируемой *лпкуери*.

</dd> </dl>

Для устройств с наложением параметр *лпкуери* указывает на структуру [**MCI \_ овли \_ Rect \_ пармс**](mci-ovly-rect-parms.md) .

## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows 2000 Professional \[только классические приложения\]<br/>                                                |
| Минимальная версия сервера<br/> | Windows 2000 Server \[только классические приложения\]<br/>                                                      |
| Заголовок<br/>                   | <dl> <dt>ммсистем. h (включает Windows. h)</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[MCI](mci.md)
</dt> <dt>

[Команды MCI](mci-commands.md)
</dt> </dl>

 

