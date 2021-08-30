---
description: Автоматическое формирование оглавления
ms.assetid: 3acb9c12-0158-4b89-87c4-4abd35ae8c2f
title: Автоматическое формирование оглавления
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: d1fd6ec833302ff24e79582a5bf3ee500d715a69e9e74910bdf9b72a2f5a64f7
ms.sourcegitcommit: e858bbe701567d4583c50a11326e42d7ea51804b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2021
ms.locfileid: "119958314"
---
# <a name="generating-a-table-of-contents-automatically"></a>Автоматическое формирование оглавления

В этом разделе показано, как использовать компонент [**генератора**](/previous-versions/ee264297(v=vs.85)) оглавлений (генератора оглавления) для автоматического создания оглавления для видеофайла.

Генератор ОГЛАВЛЕНИя — это объект мультимедиа DirectX (DMO). чтобы использовать генератор содержания DMO, создайте граф фильтра DirectX с видеофайлом в качестве источника. вставьте DMO генератора оглавления в граф фильтра и запустите граф. Затем можно получить автоматически созданную оглавление из генератора содержания DMO.

Следующая процедура предоставляет более подробные сведения.

1.  вызовите [**cocreateinstance**](/windows/win32/api/combaseapi/nf-combaseapi-cocreateinstance) , чтобы создать фильтр Graph объект (**CLSID \_ филтерграф**) и получить интерфейс [**играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) .
2.  вызовите [**cocreateinstance**](/windows/win32/api/combaseapi/nf-combaseapi-cocreateinstance) , чтобы создать объект фильтра-оболочки DMO (**CLSID \_ дмоврапперфилтер**) и получить интерфейс [**идмоврапперфилтер**](/previous-versions/windows/desktop/api/dmodshow/nn-dmodshow-idmowrapperfilter) .
3.  передавайте **\_ ктокженератордмо CLSID** в метод [**Init**](/previous-versions/windows/desktop/api/dmodshow/nf-dmodshow-idmowrapperfilter-init) фильтра оболочки DMO. это создает генератор оглавления DMO и заключает его в фильтр оболочки DMO.
4.  вызовите метод [**аддфилтер**](/windows/win32/api/strmif/nf-strmif-ifiltergraph-addfilter) интерфейса [**играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) , чтобы добавить генератор упакованных содержания DMO на граф фильтра.
    > [!Note]  
    > [**Играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) наследует от [**ифилтерграф**](/windows/win32/api/strmif/nn-strmif-ifiltergraph).

     

5.  Вызовите метод [**аддсаурцефилтер**](/windows/win32/api/strmif/nf-strmif-igraphbuilder-addsourcefilter) интерфейса [**играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) , чтобы создать фильтр источник и добавить его в граф.
6.  перечисление пин-кодов в фильтре оболочки DMO и в фильтре источника. Для этого требуется получение интерфейсов [**иенумпинс**](/windows/win32/api/strmif/nn-strmif-ienumpins) и интерфейсов [**Ипин**](/windows/win32/api/strmif/nn-strmif-ipin) .
7.  Подключение фильтр источника и фильтр оболочки путем вызова метода [**Подключение**](/windows/win32/api/strmif/nf-strmif-igraphbuilder-connect) интерфейса [**играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) .
8.  Завершите работу графа, вызвав метод [**Render**](/windows/win32/api/strmif/nf-strmif-igraphbuilder-render) интерфейса [**играфбуилдер**](/windows/win32/api/strmif/nn-strmif-igraphbuilder) .
9.  Запустите граф ([**имедиаконтрол:: Run**](/windows/win32/api/control/nf-control-imediacontrol-run)) и дождитесь его завершения ([**Имедиаевент:: ваитфоркомплетион**](/windows/win32/api/control/nf-control-imediaevent-waitforcompletion)).
10. получите интерфейс [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore) в оболочке фильтра DMO и получите значение свойства [**мфпкэй \_ токженератор \_ токреади**](/previous-versions/ee264297(v=vs.85)) . При необходимости повторите операцию, пока оглавление не будет готово.
11. Используйте интерфейс [**ипропертисторе**](/windows/win32/api/propsys/nn-propsys-ipropertystore) для получения значения свойства [**мфпкэй \_ токженератор \_ токобжект**](/previous-versions/ee264297(v=vs.85)) . Это свойство является интерфейсом [**Иток**](/windows/desktop/api/wmcodecdsp/nn-wmcodecdsp-itoc) , который представляет автоматически созданное оглавление.

В следующем коде показана процедура автоматического создания оглавления. В коде используются три вспомогательные функции ([**буилдграф**](buildgraph-method-for-generating-a-table-of-contents.md), [**рунграфандваит**](rungraphandwait-method-for-generating-a-table-of-contents.md)и [**жетток**](gettoc-method-for-generating-a-table-of-contents.md)), которые показаны на других страницах этой документации.


```C++
#include <dshow.h>
#include <dmodshow.h>
#include <wmcodecdsp.h>
#include <dmoreg.h>
#include <propsys.h>
#include <propidl.h>
#include <initguid.h>

HRESULT GetToc(IDMOWrapperFilter* pWrap, IToc** ppToc);
HRESULT RunGraphAndWait(IGraphBuilder* pGraph);
HRESULT BuildGraph(IGraphBuilder* pGraph, IDMOWrapperFilter* pWrap);

WCHAR g_sourceFile[] = L"c:\\experiment\\Seattle.wmv";

void main()
{
   HRESULT hr = E_FAIL;
   hr = CoInitialize(NULL);

   if(SUCCEEDED(hr))
   {
      IGraphBuilder* pBuilder = NULL;
      hr = CoCreateInstance(CLSID_FilterGraph, NULL, CLSCTX_INPROC_SERVER, 
         IID_IGraphBuilder, (VOID**)&pBuilder);

      if(SUCCEEDED(hr))
      {
         IDMOWrapperFilter* pWrap = NULL;
         hr = CoCreateInstance(CLSID_DMOWrapperFilter, NULL, CLSCTX_INPROC, 
            IID_IDMOWrapperFilter, (VOID**)&pWrap);

         if(SUCCEEDED(hr))
         {
            hr = pWrap->Init(CLSID_CTocGeneratorDmo, DMOCATEGORY_VIDEO_EFFECT); 

            if(SUCCEEDED(hr))
            {
               hr = BuildGraph(pBuilder, pWrap);

               if(SUCCEEDED(hr))
               {
                  hr = RunGraphAndWait(pBuilder);

                  if(SUCCEEDED(hr))
                  {
                     IToc* pToc = NULL;
                     hr = GetToc(pWrap, &pToc);

                     if(SUCCEEDED(hr))
                     {
                        // Inspect the table of contents by calling IToc methods.

                        pToc->Release();
                        pToc = NULL;
                     }
                  }
               }
            }

            pWrap->Release();
            pWrap = NULL;
         }

         pBuilder->Release();
         pBuilder = NULL;
      }

      CoUninitialize();
   }
}
```



## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Функция Буилдграф для создания оглавления](buildgraph-method-for-generating-a-table-of-contents.md)
</dt> <dt>

[Функция Жетток для создания оглавления](gettoc-method-for-generating-a-table-of-contents.md)
</dt> <dt>

[Функция Рунграфандваит для создания оглавления](rungraphandwait-method-for-generating-a-table-of-contents.md)
</dt> <dt>

[Справочное руководством по программированию синтаксического анализатора содержимого](toc-parser-programming-guide.md)
</dt> </dl>

 

 
