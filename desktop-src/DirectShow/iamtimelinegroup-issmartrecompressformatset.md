---
description: Метод Иссмартрекомпрессформатсет определяет, был ли задан для группы формат смарт-сжатия.
ms.assetid: d2b7ecc7-2348-402d-8d96-e0922e06a685
title: 'Метод Иамтимелинеграуп:: Иссмартрекомпрессформатсет (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAMTimelineGroup.IsSmartRecompressFormatSet
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: 078649fd42cd44596ff27558b29d14b6f8cbeddc
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126892096"
---
# <a name="iamtimelinegroupissmartrecompressformatset-method"></a>Метод Иамтимелинеграуп:: Иссмартрекомпрессформатсет

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`IsSmartRecompressFormatSet`Метод определяет, был ли задан формат смарт-сжатия для группы.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT IsSmartRecompressFormatSet(
   BOOL *pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*pVal* 
</dt> <dd>

Получает логическое значение, указывающее, задан ли формат сжатия. **Значение true** показывает, что был задан формат сжатия.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

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



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**Интерфейс Иамтимелинеграуп**](iamtimelinegroup.md)
</dt> <dt>

[Коды ошибок и успешности](error-and-success-codes.md)
</dt> </dl>

 

 




