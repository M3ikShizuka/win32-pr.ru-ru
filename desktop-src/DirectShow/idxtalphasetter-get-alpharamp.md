---
description: Метод Get \_ алфарамп извлекает свойство alpha пандус. Альфа-шкала — это процентная доля, на которую корректируются значения альфа в исходном изображении. Например, если альфа-пандус имеет значение 0,5, то значения альфа в изображении уменьшаются на 50%.
ms.assetid: e142a562-2e78-4418-94e9-b41320d4af57
title: 'Метод Идксталфасеттер:: get_AlphaRamp (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDxtAlphaSetter.get_AlphaRamp
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 335c227b0ac35ccd730d8ce7014b9a5c7ebc3213
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127065633"
---
# <a name="idxtalphasetterget_alpharamp-method"></a>Метод Идксталфасеттер:: Get \_ алфарамп

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_AlphaRamp`Метод извлекает свойство alpha пандус. Альфа-шкала — это процентная доля, на которую корректируются значения альфа в исходном изображении. Например, если альфа-пандус имеет значение 0,5, то значения альфа в изображении уменьшаются на 50%.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_AlphaRamp(
  [out, retval] double *pAlpha
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*палфа* \[ out, retval\]
</dt> <dd>

Получает альфа-пандус. Отрицательное значение указывает, что альфа-шкала не задана.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Возвращает значение **HRESULT** . Ниже приведены возможные значения.



| Код возврата                                                                               | Описание                          |
|-------------------------------------------------------------------------------------------|--------------------------------------|
| <dl> <dt>**\_указатель E**</dt> </dl> | **Пустой** аргумент указателя<br/> |
| <dl> <dt>**\_ОК**</dt> </dl>      | Успешное завершение<br/>                   |



 

## <a name="remarks"></a>Remarks

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Требования



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Идксталфасеттер**](idxtalphasetter.md)
</dt> </dl>

 

 




