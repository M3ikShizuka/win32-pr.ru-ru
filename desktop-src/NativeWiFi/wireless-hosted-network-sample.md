---
description: Демонстрирует использование сетевых функций, размещенных в беспроводной сети.
ms.assetid: 3da903c2-bdfa-4c1f-92e7-962551f0e08e
title: Пример беспроводной размещенной сети
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: eefc91dad883242876d7b0ddf1ec66fb92b18a79
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127461683"
---
# <a name="wireless-hosted-network-sample"></a>Пример беспроводной размещенной сети

в состав пакета средств разработки программного обеспечения (SDK) для Microsoft Windows входит пример беспроводной размещенной сети, демонстрирующий использование сетевых функций, размещенных в беспроводной сети. последняя версия Windows SDK доступна в [центре загрузки](https://www.microsoft.com/downloads/details.aspx?FamilyID=f26b1aa4-741a-433a-9be5-fa919850bdbf).

По умолчанию исходный код с примером беспроводной размещенной сети устанавливается в следующем каталоге:

**C: \\ Program files \\ Microsoft sdks \\ Windows \\ v 7.0 \\ samples \\ нетдс \\ Wlan**

Пример беспроводной размещенной сети находится в следующей папке:

**вирелесшостеднетворк**

образец беспроводной размещенной сети можно скомпилировать на Windows SDK для Windows 7. пример беспроводной размещенной сети можно запустить на Windows 7 и на Windows Server 2008 R2 с установленной службой беспроводной локальной сети.

в Windows 7 и на Windows Server 2008 R2 с установленной службой беспроводной локальной сети операционная система устанавливает виртуальное устройство, если на компьютере имеется беспроводной адаптер, поддерживающий размещенную сеть. Это виртуальное устройство обычно отображается в папке "Сетевые подключения" как "Беспроводное сетевое подключение 2" с именем устройства "адаптер мини-порта Microsoft Virtual WiFi", если компьютер имеет один беспроводной сетевой адаптер. Это виртуальное устройство используется исключительно для выполнения подключений к точке доступа к программному обеспечению (Софтап). Время существования этого виртуального устройства привязывается к физическому адаптеру беспроводной сети. Если физический адаптер беспроводной сети отключен, это виртуальное устройство также будет удалено.

Сетевые функции, размещенные в беспроводной сети, используются для запуска и отключения беспроводной размещенной сети, настройки или изменения параметров или запроса сведений.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Сведения о беспроводной размещенной сети](about-the-wireless-hosted-network.md)
</dt> <dt>

[Использование размещенной сети и общего доступа к подключению к Интернету](using-hosted-network-and-internet-connection-sharing.md)
</dt> <dt>

[**вланхостеднетворкфорцестарт**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkforcestart)
</dt> <dt>

[**вланхостеднетворкинитсеттингс**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkinitsettings)
</dt> <dt>

[**вланхостеднетворккуерипроперти**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkqueryproperty)
</dt> <dt>

[**вланхостеднетворккуерисекондарикэй**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkquerysecondarykey)
</dt> <dt>

[**вланхостеднетворккуеристатус**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkquerystatus)
</dt> <dt>

[**вланхостеднетворкрефрешсекуритисеттингс**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkrefreshsecuritysettings)
</dt> <dt>

[**вланхостеднетворксетпроперти**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworksetproperty)
</dt> <dt>

[**вланхостеднетворксетсекондарикэй**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworksetsecondarykey)
</dt> <dt>

[**вланхостеднетворкстартусинг**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkstartusing)
</dt> <dt>

[**вланхостеднетворкстопусинг**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanhostednetworkstopusing)
</dt> <dt>

[**вланрегистервиртуалстатионнотификатион**](/windows/desktop/api/Wlanapi/nf-wlanapi-wlanregistervirtualstationnotification)
</dt> </dl>

 

 



