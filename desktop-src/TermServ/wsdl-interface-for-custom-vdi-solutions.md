---
title: Интерфейс WSDL для пользовательских решений VDI
description: Разработчики могут создавать собственные веб-службы, которые управляют решениями инфраструктуры виртуальных рабочих столов (VDI).
ms.assetid: ae2dad51-be37-4311-a7c3-e99b2f41bed1
ms.tgt_platform: multiple
keywords:
- Службы удаленных рабочих столов службы удаленных рабочих столов, интерфейс WSDL для пользовательского VDI
ms.topic: article
ms.date: 05/31/2018
topic_type:
- kbArticle
api_name: ''
api_type: ''
api_location: ''
ms.openlocfilehash: 52c51c3348f41f4cd3fad990a2cc7ef94a865173
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "126890557"
---
# <a name="wsdl-interface-for-custom-vdi-solutions"></a>Интерфейс WSDL для пользовательских решений VDI

Разработчики могут создавать собственные веб-службы, которые управляют решениями инфраструктуры виртуальных рабочих столов (VDI).

начиная с Windows Server 2008 R2, клиентские компьютеры могут взаимодействовать с веб-службами, выполняющими управление виртуальными машинами с помощью подключаемого модуля фильтра VMMWebServerClient.dll. Вы можете реализовать пользовательскую веб-службу, которая работает с этим подключаемым модулем фильтра. Для взаимодействия с подключаемым модулем фильтра веб-служба должна реализовать методы, определенные в следующем файле WSDL (язык определения веб-служб).


```XML
<wsdl:definitions xmlns:soap="https://schemas.xmlsoap.org/wsdl/soap/" xmlns:wsu="https://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd" xmlns:soapenc="https://schemas.xmlsoap.org/soap/encoding/" xmlns:wsam="https://www.w3.org/2007/05/addressing/metadata" xmlns:tns="https://Microsoft.Virtualization.RDV" xmlns:wsa="https://schemas.xmlsoap.org/ws/2004/08/addressing" xmlns:wsp="https://schemas.xmlsoap.org/ws/2004/09/policy" xmlns:wsap="https://schemas.xmlsoap.org/ws/2004/08/addressing/policy" xmlns:xsd="https://www.w3.org/2001/XMLSchema" xmlns:msc="http://schemas.microsoft.com/ws/2005/12/wsdl/contract" xmlns:wsaw="https://www.w3.org/2006/05/addressing/wsdl" xmlns:soap12="https://schemas.xmlsoap.org/wsdl/soap12/" xmlns:wsa10="https://www.w3.org/2005/08/addressing" xmlns:wsx="https://schemas.xmlsoap.org/ws/2004/09/mex" targetNamespace="https://Microsoft.Virtualization.RDV" xmlns:wsdl="https://schemas.xmlsoap.org/wsdl/">
  <wsdl:types>
    <xsd:schema targetNamespace="https://Microsoft.Virtualization.RDV/Imports" xmlns:xs="https://www.w3.org/2001/XMLSchema">
      <xsd:import namespace="https://Microsoft.Virtualization.RDV" />
      <xsd:import namespace="http://schemas.microsoft.com/2003/10/Serialization/" />
      <xsd:import namespace="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" />
      <xs:element name="StartVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q1="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q1:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="StartVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="StartVMResult" xmlns:q2="http://schemas.microsoft.com/2003/10/Serialization/" type="q2:guid" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="SetLocale">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="locale" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="SetLocaleResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="SetLocaleResult" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q3="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q3:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="GetVMResult" nillable="true" xmlns:q4="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q4:VMResult" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="PlaceVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q5="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q5:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="PlaceVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="PlaceVMResult" xmlns:q6="http://schemas.microsoft.com/2003/10/Serialization/" type="q6:guid" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="JobUpdated">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="job" nillable="true" xmlns:q7="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q7:Job" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:simpleType name="NameType">
        <xs:restriction base="xs:string">
          <xs:enumeration value="COMPUTER_NAME_FQDN" />
          <xs:enumeration value="GUID" />
          <xs:enumeration value="VM_NAME" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="NameType" nillable="true" type="tns:NameType" />
      <xs:complexType name="VMResult">
        <xs:sequence>
          <xs:element minOccurs="0" name="DetailedErrorString" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="ErrorID" type="tns:VMError" />
          <xs:element minOccurs="0" name="VMList" nillable="true" type="tns:ArrayOfVM" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="VMResult" nillable="true" type="tns:VMResult" />
      <xs:simpleType name="VMError">
        <xs:restriction base="xs:string">
          <xs:enumeration value="ERROR_VM_SUCCESS" />
          <xs:enumeration value="ERROR_VM_START" />
          <xs:enumeration value="ERROR_VM_PLACEMENT" />
          <xs:enumeration value="ERROR_VM_SAVE" />
          <xs:enumeration value="ERROR_VM_RESTORE" />
          <xs:enumeration value="ERROR_VM_MISSING" />
          <xs:enumeration value="ERROR_JOB_NOT_FOUND" />
          <xs:enumeration value="ERROR_VM_LOCKED" />
          <xs:enumeration value="ERROR_VM_NO_PERMISSION" />
          <xs:enumeration value="ERROR_VM_STATE" />
          <xs:enumeration value="ERROR_SERVER_CONNECTION_LOST" />
          <xs:enumeration value="ERROR_SERVER_CONNECTION_SETUP" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="VMError" nillable="true" type="tns:VMError" />
      <xs:complexType name="ArrayOfVM">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="VM" nillable="true" type="tns:VM" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfVM" nillable="true" type="tns:ArrayOfVM" />
      <xs:complexType name="VM">
        <xs:sequence>
          <xs:element minOccurs="0" name="HostFQDN" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="HostType" type="tns:VMHostType" />
          <xs:element minOccurs="0" name="ID" type="ser:guid" />
          <xs:element minOccurs="0" name="Name" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Status" type="tns:VMStatus" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="VM" nillable="true" type="tns:VM" />
      <xs:simpleType name="VMHostType">
        <xs:restriction base="xs:string">
          <xs:enumeration value="VM_LIBRARY" />
          <xs:enumeration value="VM_HOST" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="VMHostType" nillable="true" type="tns:VMHostType" />
      <xs:simpleType name="VMStatus">
        <xs:restriction base="xs:string">
          <xs:enumeration value="VM_STATUS_UNKNOWN" />
          <xs:enumeration value="VM_STATUS_MIGRATING" />
          <xs:enumeration value="VM_STATUS_RUNNING" />
          <xs:enumeration value="VM_STATUS_HIBERNATED" />
          <xs:enumeration value="VM_STATUS_PAUSED" />
          <xs:enumeration value="VM_STATUS_STOPPED" />
          <xs:enumeration value="VM_STATUS_GUEST_BOOTED" />
          <xs:enumeration value="VM_STATUS_GUEST_REBOOTED" />
          <xs:enumeration value="VM_STATUS_GUEST_READY" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="VMStatus" nillable="true" type="tns:VMStatus" />
      <xs:complexType name="Job">
        <xs:sequence>
          <xs:element minOccurs="0" name="DetailedErrorString" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="ErrorID" type="tns:VMError" />
          <xs:element minOccurs="0" name="ID" type="ser:guid" />
          <xs:element minOccurs="0" name="Name" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Progress" type="xs:double" />
          <xs:element minOccurs="0" name="Status" type="tns:JobStatus" />
          <xs:element minOccurs="0" name="Step" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="Job" nillable="true" type="tns:Job" />
      <xs:simpleType name="JobStatus">
        <xs:restriction base="xs:string">
          <xs:enumeration value="DOES_NOT_EXISTS" />
          <xs:enumeration value="RUNNING" />
          <xs:enumeration value="FAILED" />
          <xs:enumeration value="COMPLETED" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="JobStatus" nillable="true" type="tns:JobStatus" />
    </xsd:schema>
  </wsdl:types>
  <wsdl:message name="IRDVServer_StartVM_InputMessage">
    <wsdl:part name="parameters" element="tns:StartVM" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_StartVM_OutputMessage">
    <wsdl:part name="parameters" element="tns:StartVMResponse" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_SetLocale_InputMessage">
    <wsdl:part name="parameters" element="tns:SetLocale" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_SetLocale_OutputMessage">
    <wsdl:part name="parameters" element="tns:SetLocaleResponse" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_GetVM_InputMessage">
    <wsdl:part name="parameters" element="tns:GetVM" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_GetVM_OutputMessage">
    <wsdl:part name="parameters" element="tns:GetVMResponse" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_PlaceVM_InputMessage">
    <wsdl:part name="parameters" element="tns:PlaceVM" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_PlaceVM_OutputMessage">
    <wsdl:part name="parameters" element="tns:PlaceVMResponse" />
  </wsdl:message>
  <wsdl:message name="IRDVServer_JobUpdated_OutputCallbackMessage">
    <wsdl:part name="parameters" element="tns:JobUpdated" />
  </wsdl:message>
  <wsdl:portType msc:usingSession="true" name="IRDVServer">
    <wsdl:operation msc:isInitiating="true" msc:isTerminating="false" name="StartVM">
      <wsdl:input wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/StartVM" message="tns:IRDVServer_StartVM_InputMessage" />
      <wsdl:output wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/StartVMResponse" message="tns:IRDVServer_StartVM_OutputMessage" />
    </wsdl:operation>
    <wsdl:operation msc:isInitiating="true" msc:isTerminating="false" name="SetLocale">
      <wsdl:input wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/SetLocale" message="tns:IRDVServer_SetLocale_InputMessage" />
      <wsdl:output wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/SetLocaleResponse" message="tns:IRDVServer_SetLocale_OutputMessage" />
    </wsdl:operation>
    <wsdl:operation msc:isInitiating="true" msc:isTerminating="false" name="GetVM">
      <wsdl:input wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/GetVM" message="tns:IRDVServer_GetVM_InputMessage" />
      <wsdl:output wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/GetVMResponse" message="tns:IRDVServer_GetVM_OutputMessage" />
    </wsdl:operation>
    <wsdl:operation msc:isInitiating="true" msc:isTerminating="false" name="PlaceVM">
      <wsdl:input wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/PlaceVM" message="tns:IRDVServer_PlaceVM_InputMessage" />
      <wsdl:output wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/PlaceVMResponse" message="tns:IRDVServer_PlaceVM_OutputMessage" />
    </wsdl:operation>
    <wsdl:operation msc:isInitiating="true" msc:isTerminating="false" name="JobUpdated">
      <wsdl:output wsaw:Action="https://Microsoft.Virtualization.RDV/IRDVServer/JobUpdated" message="tns:IRDVServer_JobUpdated_OutputCallbackMessage" />
    </wsdl:operation>
  </wsdl:portType>
  <wsdl:binding name="DefaultBinding_IRDVServer" type="tns:IRDVServer">
    <soap:binding transport="https://schemas.xmlsoap.org/soap/http" />
    <wsdl:operation name="StartVM">
      <soap:operation soapAction="https://Microsoft.Virtualization.RDV/IRDVServer/StartVM" style="document" />
      <wsdl:input>
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output>
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="SetLocale">
      <soap:operation soapAction="https://Microsoft.Virtualization.RDV/IRDVServer/SetLocale" style="document" />
      <wsdl:input>
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output>
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="GetVM">
      <soap:operation soapAction="https://Microsoft.Virtualization.RDV/IRDVServer/GetVM" style="document" />
      <wsdl:input>
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output>
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="PlaceVM">
      <soap:operation soapAction="https://Microsoft.Virtualization.RDV/IRDVServer/PlaceVM" style="document" />
      <wsdl:input>
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output>
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="JobUpdated">
      <soap:operation soapAction="https://Microsoft.Virtualization.RDV/IRDVServer/JobUpdated" style="document" />
      <wsdl:output>
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
  </wsdl:binding>
</wsdl:definitions>
```



Этот WSDL-файл определяет следующие методы:

-   [жетвм](#getvm)
-   [жобупдатед](#jobupdated)
-   [плацевм](#placevm)
-   [Pragma](#setlocale)
-   [StartVM](#startvm)

## <a name="getvm"></a>жетвм

Подключаемый модуль фильтра вызывает этот метод для получения сведений об указанной виртуальной машине. Он должен возвращать состояние виртуальной машины, имя узла, тип узла и идентификатор GUID.

Подключаемый модуль фильтра передает следующий элемент в метод.


```XML
      <xs:element name="GetVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q3="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q3:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



Веб-служба должна вернуть следующий элемент в подключаемый модуль фильтра.


```XML
      <xs:element name="GetVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="GetVMResult" nillable="true" xmlns:q4="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q4:VMResult" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



## <a name="jobupdated"></a>жобупдатед

Веб-служба вызывает этот метод, чтобы уведомить подключаемый модуль фильтра, что были внесены изменения в существующее задание. При реализации этого метода следует возвращать значение **\_ ОК** , если функция выполнена успешно. В случае сбоя возвратите значение **HRESULT** , указывающее на ошибку. Список распространенных кодов ошибок см. в разделе [Общие значения HRESULT](/windows/desktop/SecCrypto/common-hresult-values) .

Веб-служба передает следующий элемент подключаемому модулю фильтра.


```XML
      <xs:element name="JobUpdated">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="job" nillable="true" xmlns:q7="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q7:Job" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



## <a name="placevm"></a>плацевм

Подключаемый модуль фильтра вызывает этот метод для переноса виртуальной машины из библиотеки на главный компьютер. Метод должен порождать задание и вернуть уникальный идентификатор задания в подключаемый модуль фильтра для отслеживания. После завершения обработки веб-служба должна вызвать Жобупдатед.

Подключаемый модуль фильтра передает следующий элемент в метод.


```XML
      <xs:element name="PlaceVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q5="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q5:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



Веб-служба должна вернуть следующий элемент в подключаемый модуль фильтра.


```XML
      <xs:element name="PlaceVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="PlaceVMResult" xmlns:q6="http://schemas.microsoft.com/2003/10/Serialization/" type="q6:guid" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



## <a name="setlocale"></a>SetLocale

Подключаемый модуль фильтра вызывает этот метод, чтобы указать языковой стандарт, используемый для строк ошибок.

Подключаемый модуль фильтра передает следующий элемент в метод.


```XML
      <xs:element name="SetLocale">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="locale" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



Веб-служба должна вернуть следующий элемент в подключаемый модуль фильтра.


```XML
      <xs:element name="SetLocaleResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="SetLocaleResult" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



## <a name="startvm"></a>StartVM

Подключаемый модуль фильтра вызывает этот метод для запуска виртуальной машины на текущем хост-компьютере. Если не удается запустить виртуальную машину на текущем компьютере узла, этот метод должен перенести виртуальную машину на лучший узел, а затем запустить ее. Метод должен порождать задание и вернуть уникальный идентификатор задания в подключаемый модуль фильтра для отслеживания. После завершения обработки веб-служба должна вызвать Жобупдатед.

Подключаемый модуль фильтра передает следующий элемент в метод.


```XML
      <xs:element name="StartVM">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="name" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="type" xmlns:q1="https://schemas.datacontract.org/2004/07/Microsoft.Virtualization.RDV" type="q1:NameType" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



Веб-служба должна вернуть следующий элемент в подключаемый модуль фильтра.


```XML
      <xs:element name="StartVMResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="StartVMResult" xmlns:q2="http://schemas.microsoft.com/2003/10/Serialization/" type="q2:guid" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
```



 

 