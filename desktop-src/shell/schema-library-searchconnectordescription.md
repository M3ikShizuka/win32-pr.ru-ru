---
description: '&lt;Элемент сеарчконнектордескриптион &gt; является элементом контейнера верхнего уровня определения соединителя поиска.'
ms.assetid: 383CAA20-56CA-4bdc-AC79-E57A1D59785C
title: Элемент Сеарчконнектордескриптион (схема библиотеки)
ms.topic: article
ms.date: 05/31/2018
ms.openlocfilehash: eddf7c2795f5c87009bc17b5fa3899d339ceed3c
ms.sourcegitcommit: 61a4c522182aa1cacbf5669683d9570a3bf043b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "122885970"
---
# <a name="searchconnectordescription-element-library-schema"></a>Элемент Сеарчконнектордескриптион (схема библиотеки)

&lt;Элемент сеарчконнектордескриптион &gt; является элементом контейнера верхнего уровня определения соединителя поиска. &lt;элемент сеарчконнектордескриптион &gt; является расширением &lt; &gt; типа элемента сеарчконнектордескриптионтипе, связанного с Windows федеративными соединителями поиска. однако соединители поиска для Windows федеративного поиска или обработчиков протоколов в библиотеке использовать нельзя.

## <a name="syntax"></a>Синтаксис

``` syntax
<!-- searchConnectorDescription -->
<?xml version="1.0" encoding="UTF-8"?>
<xs:schema xmlns:xs="https://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" attributeFormDefault="unqualified">
   <xs:complexType name="searchConnectorDescriptionType">
      <xs:all>
         <xs:element name="isSearchOnlyItem" type="xs:boolean" default="false" minOccurs="0"/>
         <xs:element name="isDefaultSaveLocation" type="xs:boolean" minOccurs="0"/>
         <xs:element name="isDefaultNonOwnerSaveLocation" type="xs:boolean" minOccurs="0"/
         <xs:element name="description" type="xs:string" minOccurs="0"/>
         <xs:element name="iconReference" type="xs:string" minOccurs="0"/>
         <xs:element name="imageLink" minOccurs="0">
            <xs:complexType>
               <xs:sequence>
                  <xs:element name="url" type="xs:anyURI"/>
               </xs:sequence>
            </xs:complexType>
         </xs:element>
         <xs:element name="author" type="xs:string" minOccurs="0"/>
         <xs:element name="dateCreated" type="xs:dateTime" minOccurs="0"/>
         <xs:element name="templateInfo" minOccurs="0">
            <xs:complexType>
               <xs:all>
                  <xs:element name="folderType" minOccurs="0"/>
               </xs:all>
            </xs:complexType>
         </xs:element>
         <xs:element name="simpleLocation" type="shellLinkType" minOccurs="0"/>
         <xs:element name="locationProvider" minOccurs="0">
            <xs:complexType>
               <xs:all>
                  <xs:element name="propertyBag" type="propertyStoreType" minOccurs="0"/>
               </xs:all>
               <xs:attribute name="clsid" use="required"/>
               <xs:attribute name="codebase" type="xs:string"/>
            </xs:complexType>
         </xs:element>
         <xs:element name="scope" minOccurs="0">
            <xs:complexType>
               <xs:sequence minOccurs="0">
                  <xs:element name="scopeItem" maxOccurs="unbounded">
                     <xs:complexType>
                        <xs:all>
                           <xs:element name="mode" default="Include">
                              <xs:simpleType>
                                 <xs:restriction base="xs:string">
                                    <xs:enumeration value="Include"/>
                                    <xs:enumeration value="Exclude"/>
                                 </xs:restriction>
                              </xs:simpleType>
                           </xs:element>
                           <xs:element name="depth" default="Shallow" minOccurs="0">
                              <xs:simpleType>
                                 <xs:restriction base="xs:string">
                                    <xs:enumeration value="Shallow"/>
                                    <xs:enumeration value="Deep"/>
                                 </xs:restriction>
                              </xs:simpleType>
                           </xs:element>
                           <xs:element name="url" type="xs:anyURI"/>
                        </xs:all>
                     </xs:complexType>
                  </xs:element>
               </xs:sequence>
            </xs:complexType>
         </xs:element>
         <xs:element name="propertyStore" type="propertyStoreType" minOccurs="0"/>
         <xs:element name="includeInStartMenuScope" type="xs:boolean" default="false" minOccurs="0"/>
         <xs:element name="domain" type="xs:string" minOccurs="0"/>
         <xs:element name="supportsAdvancedQuerySyntax" type="xs:boolean" default="false" minOccurs="0"/>
         <xs:element name="isIndexed" type="xs:boolean" minOccurs="0"/>
      </xs:all>
      <xs:attribute name="publisher" type="xs:string"/>
      <xs:attribute name="product" type="xs:string"/>
   </xs:complexType>
</xs:schema>
```

## <a name="element-information"></a>Сведения об элементе

см. документацию по схеме в [Windowsном поиске](/previous-versions/bb268030(v=msdn.10)) .



| Родительский элемент                                                                                               | Дочерние элементы                        |
|--------------------------------------------------------------------------------------------------------------|---------------------------------------|
| [Элемент Сеарчконнектордескриптионлист (схема библиотеки)](schema-library-searchconnectordescriptionlist.md) | <Иссеарчонли. TEM>             |
|                                                                                                              | &lt;Описание&gt;                   |
|                                                                                                              | &lt;иконреференце&gt;                 |
|                                                                                                              | &lt;имажелинк&gt;                     |
|                                                                                                              | &lt;календаря&gt;                        |
|                                                                                                              | &lt;dateCreated&gt;                   |
|                                                                                                              | &lt;темплатеинфо&gt;                  |
|                                                                                                              | &lt;локатионпровидер&gt;              |
|                                                                                                              | &lt;область&gt;                         |
|                                                                                                              | &lt;пропертисторе&gt;                 |
|                                                                                                              | &lt;domain&gt;                        |
|                                                                                                              | &lt;суппортсадванцедкуерисинтакс&gt;   |
|                                                                                                              | &lt;исдефаултсавелокатион&gt;         |
|                                                                                                              | &lt;исдефаултноновнерсавелокатион&gt; |
|                                                                                                              | &lt;Индексируется&gt;                     |
|                                                                                                              | &lt;симплелокатион&gt;                |
|                                                                                                              | &lt;инклудеинстартмену&gt;            |



 

## <a name="attributes"></a>Атрибуты



| Атрибут | Описание                                                                      |
|-----------|----------------------------------------------------------------------------------|
| publisher | Необязательный элемент. Отображаемое имя издателя, предоставляющего соединитель поиска.      |
| product   | Необязательный элемент. Отображаемое имя продукта, к которому применяется соединитель поиска. |



 

## <a name="remarks"></a>Комментарии

&lt;элемент сеарчконнектордескриптион &gt; библиотеки использует то же определение схемы, что и сеарчконнектордескриптион, &lt; &gt; для Windows федеративного поиска. несмотря на то что они используют одни и те же схемы, соединители поиска для Windows федеративного поиска не могут быть добавлены в библиотеку.

## <a name="related-topics"></a>Связанные темы

<dl> <dt>

[Схема описания библиотеки](library-schema-entry.md)
</dt> <dt>

[Схема описания соединителя поиска](../search/search-sconn-desc-schema-entry.md)
</dt> </dl>

 

 
