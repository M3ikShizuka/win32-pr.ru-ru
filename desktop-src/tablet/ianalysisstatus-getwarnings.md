---
description: Извлекает коллекцию Ианалисисварнингс, которая описывает все ошибки и предупреждения, созданные операцией анализа.
ms.assetid: fe1258a1-c9a9-4090-a458-f5f09371057a
title: Метод Ианалисисстатус::-Warnings (Иаком. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- IAnalysisStatus.GetWarnings
api_type:
- COM
api_location:
- IACom.dll
ms.openlocfilehash: f3a5ba2c7c6e0ab586861d209ebb7cae3761af4e
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127572455"
---
# <a name="ianalysisstatusgetwarnings-method"></a>Метод Ианалисисстатус:: "Warnings"

Извлекает коллекцию [**ианалисисварнингс**](ianalysiswarnings.md) , которая описывает все ошибки и предупреждения, созданные операцией анализа.

## <a name="syntax"></a>Синтаксис


```C++
HRESULT GetWarnings(
  [out] IAnalysisWarnings **ppAnalysisWarnings
);
```



## <a name="parameters"></a>Параметры

<dl> <dt>

*ппаналисисварнингс* \[ заполняет\]
</dt> <dd>

Указатель на коллекцию [**ианалисисварнингс**](ianalysiswarnings.md) , которая описывает все ошибки и предупреждения, созданные операцией анализа.

</dd> </dl>

## <a name="return-value"></a>Возвращаемое значение

Описание возвращаемых значений см. в разделе [классы и интерфейсы — анализ рукописного ввода](classes-and-interfaces---ink-analysis.md).

## <a name="remarks"></a>Комментарии

> [!Caution]  
> Вызовите [**IUnknown:: Release**](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) в \* *ппаналисисварнингс* , если предупреждение больше не требуется.

 

## <a name="examples"></a>Примеры

В следующем примере показана структура обработчика событий для события [**\_ ианалисисевентс:: Results**](-ianalysisevents-results.md) . Обработчик проверяет [**ианалисисстатус:: Success**](ianalysisstatus-issuccessful.md). Если операция анализа создает предупреждения, обработчик выполняет итерацию по коллекции объектов [**ианалисисварнинг**](ianalysiswarning.md) .


```C++
// _IAnalysisEvents::Results event handler.
STDMETHODIMP CMyClass::Results(
    IInkAnalyzer *pInkAnalyzer,
    IAnalysisStatus *pAnalysisStatus)
{
    // Check the status of the analysis operation.
    VARIANT_BOOL bResult = VARIANT_FALSE;
    HRESULT hr = pAnalysisStatus->IsSuccessful(&bResult);

    if( SUCCEEDED(hr) )
    {
        if( bResult )
        {
            // Insert code that handles a successful result.
        }
        else
        {
            // Get the analysis warnings.
            IAnalysisWarnings* pAnalysisWarnings = NULL;
            hr = pAnalysisStatus->GetWarnings(&pAnalysisWarnings);
            if (SUCCEEDED(hr))
            {
                // Iterate through the warning collection.
                ULONG warningCount = 0;
                hr = pAnalysisWarnings->GetCount(&warningCount);
                if (SUCCEEDED(hr))
                {
                    IAnalysisWarning *pAnalysisWarning = NULL;
                    AnalysisWarningCode analysisWarningCode;
                    for (ULONG index=0; index<warningCount; index++)
                    {
                        // Get an analysis warning.
                        hr = pAnalysisWarnings->GetAnalysisWarning(
                            index, &pAnalysisWarning);

                        if (SUCCEEDED(hr))
                        {
                            // Get the warning code for the warning.
                            hr = pAnalysisWarning->GetWarningCode(
                                &analysisWarningCode);

                            if (SUCCEEDED(hr))
                            {
                                // Insert code that handles each
                                // analysis warning.
                            }
                        }

                        // Release this reference to the analysis warning.
                        if (pAnalysisWarning != NULL)
                        {
                            pAnalysisWarning->Release();
                            pAnalysisWarning = NULL;
                        }

                        if (FAILED(hr))
                        {
                            break;
                        }
                    }
                }
            }

            // Release this reference to the analysis warnings collection.
            if (pAnalysisWarnings != NULL)
            {
                pAnalysisWarnings->Release();
                pAnalysisWarnings = NULL;
            }
        }
    }
    return hr;
}
```



## <a name="requirements"></a>Требования



| Требование | Значение |
|-------------------------------------|---------------------------------------------------------------------------------------------------------------|
| Минимальная версия клиента<br/> | Windows XP Tablet PC Edition \[ только классические приложения\]<br/>                                                 |
| Минимальная версия сервера<br/> | Ни одна версия не поддерживается<br/>                                                                                     |
| Заголовок<br/>                   | <dl> <dt>Иаком. h (также требуется Иаком \_ i. c)</dt> </dl> |
| DLL<br/>                      | <dl> <dt>IACom.dll</dt> </dl>                          |



## <a name="see-also"></a>См. также раздел

<dl> <dt>

[**ианалисисстатус**](ianalysisstatus.md)
</dt> <dt>

[**ианалисисварнингс**](ianalysiswarnings.md)
</dt> <dt>

[**ианалисисварнинг**](ianalysiswarning.md)
</dt> <dt>

[**аналисисварнингкоде**](/windows/desktop/tablet/analysiswarningcode)
</dt> <dt>

[Справочник по анализу рукописного ввода](ink-analysis-reference.md)
</dt> </dl>

 

