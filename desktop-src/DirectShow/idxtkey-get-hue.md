---
description: Метод получения \_ оттенок получает значение оттенка, по которому следует подключаться. Это свойство применяется только в том случае, если тип ключа — ДКСТКЭЙный \_ тон.
ms.assetid: d37fedd6-f29f-4f16-821b-c5f8520c4e12
title: 'Метод Идксткэй:: get_Hue (Кедит. h)'
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IDxtKey.get_Hue
api_type:
- COM
api_location:
- strmiids.lib
- strmiids.dll
ms.openlocfilehash: a003dc0cba632e354a0188571f87266902ce1396adcabb862aee258e5701f2cf
ms.sourcegitcommit: e6600f550f79bddfe58bd4696ac50dd52cb03d7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119997484"
---
# <a name="idxtkeyget_hue-method"></a>Метод Идксткэй:: Get \_ оттенок

> [!Note]  
> \[Не рекомендуется. Этот API может быть удален из будущих выпусков Windows.\]

 

`get_Hue`Метод получает значение оттенка, по которому следует подключаться. Это свойство применяется только в том случае, если тип ключа — ДКСТКЭЙный \_ тон.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT get_Hue(
  [out, retval] int *pVal
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*Pval* \[ out, retval\]
</dt> <dd>

Получает значение оттенка ключа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Если этот метод завершается успешно, возвращается значение **S \_ ОК**. В противном случае возвращается код ошибки **HRESULT** .

## <a name="remarks"></a>Remarks

> [!Note]  
> Файл заголовка Кедит. h несовместим с заголовками Direct3D позднее версии 7.

 

> [!Note]  
> чтобы получить кедит. h, скачайте [обновление Microsoft Windows SDK для Windows Vista и платформа .NET Framework 3,0](https://msdn.microsoft.com/windowsvista/bb980924.aspx). кедит. h недоступен в Microsoft Windows SDK для Windows 7 и платформа .NET Framework 3,5 с пакетом обновления 1 (sp1).

 

## <a name="requirements"></a>Requirements (Требования)



| Требование | Значение |
|--------------------|-----------------------------------------------------------------------------------------|
| Заголовок<br/>  | <dl> <dt>Кедит. h</dt> </dl>      |
| Библиотека<br/> | <dl> <dt>Стрмиидс. lib</dt> </dl> |



## <a name="see-also"></a>См. также

<dl> <dt>

[**Интерфейс Идксткэй**](idxtkey.md)
</dt> <dt>

[**Идксткэй:: Get \_ KeyType**](idxtkey-get-keytype.md)
</dt> </dl>

 

 




