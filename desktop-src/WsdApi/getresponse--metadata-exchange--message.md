---
description: WS-Transfer сообщение, используемое для ответа на запрос метаданных.
ms.assetid: aff05317-35db-4ea6-9692-1e09e4682fe7
title: сообщение о выклике (метаданные Exchange)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: 6b22782ae8b00530f6c857d867694be43b32e495
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127567191"
---
# <a name="getresponse-metadata-exchange-message"></a>сообщение о выклике (метаданные Exchange)

Сообщение GetResponse — это WS-Transfer сообщение, используемое для ответа на запрос метаданных. Дополнительные сведения о сообщениях GetResponse см. в разделе 3,1 [спецификации WS-передач](https://specs.xmlsoap.org/ws/2004/09/transfer/WS-Transfer.pdf).

Любое приложение DPWS, отправляющее сообщения [Get](get--metadata-exchange--http-request-and-message.md) , получает сообщения GetResponse.

> [!Note]  
> В этом разделе показан пример сообщения DPWS, созданного WSDAPI-клиентами и узлами. WSDAPI будет анализировать и принимать другие сообщения, соответствующие DPWS, которые не соответствуют этому примеру. Не используйте этот пример для проверки взаимодействия DPWS. Используйте вместо него [базовое средство взаимодействия WSDAPI (всдбит)](https://msdn.microsoft.com/library/cc264250.aspx) .

 

В следующем сообщении SOAP показан пример сообщения GetResponse.

``` syntax
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope
    xmlns:soap="https://www.w3.org/2003/05/soap-envelope"
    xmlns:wsa="https://schemas.xmlsoap.org/ws/2004/08/addressing"
    xmlns:wsx="https://schemas.xmlsoap.org/ws/2004/09/mex"
    xmlns:wsdp="https://schemas.xmlsoap.org/ws/2006/02/devprof"
    xmlns:sim="https://schemas.example.org/SimpleService"
    xmlns:att="https://schemas.example.org/AttachmentService"
    xmlns:eve="https://schemas.example.org/EventingService">
<soap:Header>
    <wsa:To>
        https://schemas.xmlsoap.org/ws/2004/08/addressing/role/anonymous
    </wsa:To>
    <wsa:Action>
        https://schemas.xmlsoap.org/ws/2004/09/transfer/GetResponse
    </wsa:Action>
    <wsa:MessageID>
        urn:uuid:119dcdf5-fc0d-4d40-bf1f-de52dc292744
    </wsa:MessageID>
    <wsa:RelatesTo>
        urn:uuid:027bec45-c37c-466c-936c-68f648abe2bb
    </wsa:RelatesTo>
</soap:Header>
<soap:Body>
    <wsx:Metadata>
        <wsx:MetadataSection Dialect="https://schemas.xmlsoap.org/ws/2006/02/devprof/ThisDevice">
            <wsdp:ThisDevice>
                <wsdp:FriendlyName>
                    WSDAPI Basic Interop Server
                </wsdp:FriendlyName>
                <wsdp:FirmwareVersion>alpha</wsdp:FirmwareVersion>
                <wsdp:SerialNumber>1</wsdp:SerialNumber>
            </wsdp:ThisDevice>
        </wsx:MetadataSection>
        <wsx:MetadataSection Dialect="https://schemas.xmlsoap.org/ws/2006/02/devprof/ThisModel">
            <wsdp:ThisModel>
                <wsdp:Manufacturer>
                    Microsoft
                </wsdp:Manufacturer>
                <wsdp:ManufacturerUrl>
                    https://www.microsoft.com/
                </wsdp:ManufacturerUrl>
                <wsdp:ModelName>
                    WSDAPI Interop device
                </wsdp:ModelName>
                <wsdp:ModelNumber>0.1</wsdp:ModelNumber>
                <wsdp:ModelUrl>
                    https://www.microsoft.com/
                </wsdp:ModelUrl>
                <wsdp:PresentationUrl>
                    https://www.microsoft.com/
                </wsdp:PresentationUrl>
            </wsdp:ThisModel>
        </wsx:MetadataSection>
        <wsx:MetadataSection Dialect="https://schemas.xmlsoap.org/ws/2006/02/devprof/Relationship">
            <wsdp:Relationship Type="https://schemas.xmlsoap.org/ws/2006/02/devprof/host">
                <wsdp:Host>
                    <wsa:EndpointReference>
                        <wsa:Address>
                            urn:uuid:37f86d35-e6ac-4241-964f-1d9ae46fb366
                        </wsa:Address>
                    </wsa:EndpointReference>
                    <wsdp:Types>sim:SimpleDeviceType</wsdp:Types>
                    <wsdp:ServiceId>
                        https://testdevice.interop/SimpleDevice
                    </wsdp:ServiceId>
                </wsdp:Host>
                <wsdp:Hosted>
                    <wsa:EndpointReference>
                        <wsa:Address>
                            https://192.168.0.2:5357/37f86d35-e6ac-4241-964f-1d9ae46fb366
                        </wsa:Address>
                    </wsa:EndpointReference>
                    <wsdp:Types>sim:SimpleService</wsdp:Types>
                    <wsdp:ServiceId>
                        https://testdevice.interop/SimpleService1
                    </wsdp:ServiceId>
                </wsdp:Hosted>
            </wsdp:Relationship>
        </wsx:MetadataSection>
    </wsx:Metadata>
</soap:Body>
</soap:Envelope>
```

Сообщение GetResponse имеет следующие фокусы.



<table>
<colgroup>
<col  />
<col  />
<col  />
</colgroup>
<thead>
<tr class="header">
<th>точка фокусировки;</th>
<th>XML</th>
<th>Описание</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>GetResponse</td>
<td><pre class="syntax" data-space="preserve"><code>&lt;wsa:Action&gt;
    https://schemas.xmlsoap.org/ws/2004/09/transfer/GetResponse
&lt;/wsa:Action&gt;</code></pre></td>
<td>Действие SOAP GetResponse определяет сообщение как сообщение с ответом.</td>
</tr>
<tr class="even">
<td>RelatesTo</td>
<td><pre class="syntax" data-space="preserve"><code>&lt;wsa:RelatesTo&gt;
    urn:uuid:027bec45-c37c-466c-936c-68f648abe2bb
&lt;/wsa:RelatesTo&gt;</code></pre></td>
<td>Идентификатор сообщения, на которое отвечает устройство. Этот заголовок соответствует идентификатору MessageID в сообщении <a href="get--metadata-exchange--http-request-and-message.md">Get</a> .</td>
</tr>
<tr class="odd">
<td>Адрес</td>
<td><pre class="syntax" data-space="preserve"><code>&lt;wsa:Address&gt;
    https://192.168.0.2:5357/37f86d35-e6ac-4241-964f-1d9ae46fb366
&lt;/wsa:Address&gt;</code></pre></td>
<td>Содержит адрес конечной точки служб, размещенных на этом устройстве.</td>
</tr>
</tbody>
</table>



 

## <a name="related-topics"></a>Связанные разделы

<dl> <dt>

[обнаружение и метаданные Exchange сообщения](discovery-and-metadata-exchange-message-patterns.md)
</dt> <dt>

[Получение сообщения](get--metadata-exchange--http-request-and-message.md)
</dt> </dl>

 

 



