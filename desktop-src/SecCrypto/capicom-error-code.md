---
description: Определяет коды ошибок, возвращаемые CAPICOM.
ms.assetid: e72b8290-b482-4629-8b87-5a15677865a6
title: Перечисление CAPICOM_ERROR_CODE (CAPICOM. h)
ms.topic: reference
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- CAPICOM_ERROR_CODE
api_type:
- HeaderDef
api_location:
- Capicom.h
ms.openlocfilehash: abdd2556ace3e3c3c82ccdeedc907d77f9ce1702
ms.sourcegitcommit: d75fc10b9f0825bbe5ce5045c90d4045e3c53243
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2021
ms.locfileid: "127171175"
---
# <a name="capicom_error_code-enumeration"></a>\_ \_ Перечисление кода ошибки CAPICOM

Тип перечисления " **CAPICOM \_ \_ Code Error** " определяет коды ошибок, возвращаемые CAPICOM.

> [!Note]  
> Visual Basic Ошибки в выпуске сценариев возвращают значение **Err. Number** больше нуля. Для этих ошибок значения **Err. Description** содержат сведения о причине ошибки. помимо Visual Basic ошибок выпуска сценариев, CAPICOM errors возвращает коды, определенные **\_ \_ кодом ошибки capicom**.

 

## <a name="members"></a>Элементы




| Член | Описание | Значение | 
|--------|-------------|-------|
| <strong>CAPICOM_E_ENCODE_INVALID_TYPE</strong> | Использован недопустимый тип кодирования.<br /> В следующем списке приведены допустимые типы кодировки.<ul><li>CAPICOM_ENCODE_ANY</li><li>CAPICOM_ENCODE_BASE64</li><li>CAPICOM_ENCODE_BINARY</li></ul><br /> | 0x80880100 | 
| <strong>CAPICOM_E_EKU_INVALID_OID</strong> | Свойство <a href="eku-oid.md"><strong>OID</strong></a> объекта <a href="eku.md"><strong>EKU</strong></a> не может быть задано, так как свойство <a href="eku-name.md"><strong>Name</strong></a> не имеет значение CAPICOM_EKU_OTHER.<br /> Присвойте свойству <a href="eku-name.md"><strong>Name</strong></a> значение CAPICOM_EKU_OTHER, прежде чем задавать свойство <a href="eku-oid.md"><strong>OID</strong></a> .<br /> | 0x80880200 | 
| <strong>CAPICOM_E_EKU_OID_NOT_INITIALIZED</strong> | Свойство <a href="eku-oid.md"><strong>OID</strong></a> объекта <a href="eku.md"><strong>EKU</strong></a> не инициализировано. <br /> Либо задайте для свойства <a href="eku-name.md"><strong>Name</strong></a> значение, отличное от CAPICOM_EKU_OTHER, либо установите свойство <strong>Name</strong> в CAPICOM_EKU_OTHER и свойство <a href="eku-oid.md"><strong>OID</strong></a> в качестве значения.<br /> | 0x80880201 | 
| <strong>CAPICOM_E_CERTIFICATE_NOT_INITIALIZED</strong> | Объект <a href="certificate.md"><strong>сертификата</strong></a> не инициализирован.<br /> Как правило, этот код ошибки возвращается, когда экземпляр объекта <a href="certificate.md"><strong>сертификата</strong></a> создается, но не связан с цифровым сертификатом. Чтобы связать объект с цифровым сертификатом, либо назначьте его существующему объекту <strong>сертификата</strong> , либо вызовите метод <a href="certificate-import.md"><strong>Import</strong></a> .<br /> | 0x80880210 | 
| <strong>CAPICOM_E_CERTIFICATE_NO_PRIVATE_KEY</strong> | У объекта <a href="certificate.md"><strong>сертификата</strong></a> нет связанного закрытого ключа.<br /> Этот код ошибки возвращается при попытке подписать данные с помощью закрытого ключа подписавший, но объект <a href="certificate.md"><strong>сертификата</strong></a> , связанный с объектом- <a href="signer.md"><strong>подписавшим</strong></a> , не может использоваться для операции подписывания.<br /> | 0x80880211 | 
| <strong>CAPICOM_E_CHAIN_NOT_BUILT</strong> | Объект <a href="chain.md"><strong>цепочки</strong></a> не инициализирован. <br /> Чтобы инициализировать объект <a href="chain.md"><strong>цепочки</strong></a> , вызовите метод <a href="chain-build.md"><strong>Build</strong></a> .<br /> | 0x80880220 | 
| <strong>CAPICOM_E_STORE_NOT_OPENED</strong> | Объект <a href="store.md"><strong>Store</strong></a> не был инициализирован. <br /> Чтобы инициализировать объект <a href="store.md"><strong>Store</strong></a> , вызовите метод <a href="store-open.md"><strong>Open</strong></a> .<br /> | 0x80880230 | 
| <strong>CAPICOM_E_STORE_EMPTY</strong> | Объект <a href="store.md"><strong>хранилища</strong></a> не содержит объектов <a href="certificate.md"><strong>сертификата</strong></a> .<br /> | 0x80880231 | 
| <strong>CAPICOM_E_STORE_INVALID_OPEN_MODE</strong> | Параметр <em>OpenMode</em> метода <a href="store-open.md"><strong>Store. Open</strong></a> не содержит допустимое значение CAPICOM_STORE_OPEN_MODE.<br /> В следующем списке приведены допустимые значения CAPICOM_STORE_OPEN_MODE.<ul><li>CAPICOM_STORE_OPEN_READ_ONLY</li><li>CAPICOM_STORE_OPEN_READ_WRITE</li><li>CAPICOM_STORE_OPEN_MAXIMUM_ALLOWED</li><li>CAPICOM_STORE_OPEN_EXISTING_ONLY</li><li>CAPICOM_STORE_OPEN_INCLUDE_ARCHIVED</li></ul><br /> | 0x80880232 | 
| <strong>CAPICOM_E_STORE_INVALID_SAVE_AS_TYPE</strong> | Недопустимое значение <em>SaveAs</em> , передаваемое методу <a href="store-export.md"><strong>Export</strong></a> объекта <a href="store.md"><strong>Store</strong></a> . <br /> В следующем списке приведены допустимые значения <em>SaveAs</em> :<ul><li>CAPICOM_STORE_SAVE_AS_SERIALIZED</li><li>CAPICOM_STORE_SAVE_AS_PKCS7</li></ul><br /> | 0x80880233 | 
| <strong>CAPICOM_E_ATTRIBUTE_NAME_NOT_INITIALIZED</strong> | Свойство <a href="attribute-name.md"><strong>Name</strong></a> объекта <a href="attribute.md"><strong>Attribute</strong></a> не было инициализировано. <br /> Задайте свойство <a href="attribute-name.md"><strong>Name</strong></a> .<br /> | 0x80880240 | 
| <strong>CAPICOM_E_ATTRIBUTE_VALUE_NOT_INITIALIZED</strong> | Свойство <a href="attribute-value.md"><strong>value</strong></a> объекта <a href="attribute.md"><strong>атрибута</strong></a> не было инициализировано. <br /> Задайте свойство <a href="attribute-value.md"><strong>value</strong></a> .<br /> | 0x80880241 | 
| <strong>CAPICOM_E_ATTRIBUTE_INVALID_NAME</strong> | Недопустимое свойство <a href="attribute-name.md"><strong>Name</strong></a> объекта <a href="attribute.md"><strong>Attribute</strong></a> . <br /> В следующем списке приведены допустимые имена атрибутов.<ul><li>CAPICOM_AUTHENTICATED_ATTRIBUTE_SIGNING_TIME</li><li>CAPICOM_AUTHENTICATED_ATTRIBUTE_DOCUMENT_NAME</li><li>CAPICOM_AUTHENTICATED_ATTRIBUTE_DOCUMENT_DESCRIPTION</li></ul><br /> | 0x80880242 | 
| <strong>CAPICOM_E_ATTRIBUTE_INVALID_VALUE</strong> | Свойство <a href="attribute-value.md"><strong>value</strong></a> объекта <a href="attribute.md"><strong>атрибута</strong></a> является недопустимым, так как тип данных не соответствует типу данных, указанному свойством <strong>Name</strong> . <br /> Например, если свойство <a href="attribute-value.md"><strong>Name</strong></a> имеет значение CAPICOM_AUTHENTICATED_ATTRIBUTE_SIGNING_TIME, то тип данных должен быть <strong>Date</strong>.<br /> | 0x80880243 | 
| <strong>CAPICOM_E_SIGNER_NOT_INITIALIZED</strong> | Объект <a href="signer.md"><strong>подписавший</strong></a> не инициализирован. <br /> Чтобы инициализировать объект <a href="signer.md"><strong>Sign</strong></a> , задайте свойство <a href="signer-certificate.md"><strong>Certificate</strong></a> .<br /> | 0x80880250 | 
| <strong>CAPICOM_E_SIGNER_NOT_FOUND</strong> | Не удается найти подписывание в объекте <a href="signeddata.md"><strong>сигнеддата</strong></a> . <br /> Как правило, это не происходит при использовании объекта <a href="signeddata.md"><strong>сигнеддата</strong></a> , созданного CAPICOM; Однако если объект <strong>сигнеддата</strong> был создан сторонним продуктом, сертификат лица может не включаться в структуру PKCS #7.<br /> | 0x80880251 | 
| <strong>CAPICOM_E_SIGNER_NO_CHAIN</strong> | Не удалось найти объект <a href="chain.md"><strong>цепочки</strong></a> в объекте- <a href="signer.md"><strong>подписавшем</strong></a> .<br /> | 0x80880252//v 2.0 | 
| <strong>CAPICOM_E_SIGNER_INVALID_USAGE</strong> | Предпринята попытка использовать подписывающий недопустимым образом.<br /> | 0x80880253 //v2.0 | 
| <strong>CAPICOM_E_SIGN_NOT_INITIALIZED</strong> | Объект <a href="signeddata.md"><strong>сигнеддата</strong></a> не инициализирован. <br /> Чтобы инициализировать объект <a href="signeddata.md"><strong>сигнеддата</strong></a> , задайте свойство <a href="signeddata-content.md"><strong>Content</strong></a> или вызовите метод <a href="signeddata-verify.md"><strong>Verify</strong></a> .<br /> | 0x80880260 | 
| <strong>CAPICOM_E_SIGN_INVALID_TYPE</strong> | Объект <a href="signeddata.md"><strong>сигнеддата</strong></a> содержит недопустимый тип. <br /> Как правило, это происходит при попытке проверить упакованное сообщение с помощью объекта <a href="signeddata.md"><strong>сигнеддата</strong></a> или наоборот.<br /> | 0x80880261 | 
| <strong>CAPICOM_E_SIGN_NOT_SIGNED</strong> | Объект <a href="signeddata.md"><strong>сигнеддата</strong></a> не подписан. <br /> Чтобы подписать объект <a href="signeddata.md"><strong>сигнеддата</strong></a> , вызовите метод <a href="signeddata-sign.md"><strong>Sign</strong></a> .<br /> | 0x80880262 | 
| <strong>CAPICOM_E_INVALID_ALGORITHM</strong> | Недопустимое значение алгоритма для свойства <a href="algorithm-name.md"><strong>Name</strong></a> объекта <a href="algorithm.md"><strong>Algorithm</strong></a> . <br /> В следующем списке показаны допустимые значения алгоритма для свойства <a href="algorithm-name.md"><strong>Name</strong></a> :<ul><li>CAPICOM_ENCRYPTION_ALGORITHM_RC2</li><li>CAPICOM_ENCRYPTION_ALGORITHM_RC4</li><li>CAPICOM_ENCRYPTION_ALGORITHM_DES</li><li>CAPICOM_ENCRYPTION_ALGORITHM_3DES</li></ul><br /> | 0x80880270 | 
| <strong>CAPICOM_E_INVALID_KEY_LENGTH</strong> | Недопустимое значение длины ключа для свойства <a href="algorithm-keylength.md"><strong>keylength</strong></a> объекта <a href="algorithm.md"><strong>Algorithm</strong></a> . <br /> В следующем списке приведены допустимые значения длины ключа для свойства <a href="algorithm-keylength.md"><strong>keylength</strong></a> :<ul><li>CAPICOM_ENCRYPTION_KEY_LENGTH_MAXIMUM</li><li>CAPICOM_ENCRYPTION_KEY_LENGTH_40_BITS</li><li>CAPICOM_ENCRYPTION_KEY_LENGTH_56_BITS</li><li>CAPICOM_ENCRYPTION_KEY_LENGTH_128_BITS</li></ul><br /> | 0x80880271 | 
| <strong>CAPICOM_E_ENVELOP_NOT_INITIALIZED</strong> | Объект <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> не инициализирован. <br /> Чтобы инициализировать объект <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> , необходимо либо задать свойство <a href="envelopeddata-content.md"><strong>Content</strong></a> , либо вызвать метод <a href="envelopeddata-decrypt.md"><strong>дешифровки</strong></a> .<br /> | 0x80880280 | 
| <strong>CAPICOM_E_ENVELOP_INVALID_TYPE</strong> | Объект <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> содержит недопустимый тип. <br /> Обычно это происходит при попытке проверить подписанное сообщение с помощью объекта <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> или наоборот.<br /> | 0x80880281 | 
| <strong>CAPICOM_E_ENVELOP_NO_RECIPIENT</strong> | При вызове метода <a href="envelopeddata-encrypt.md"><strong>Encrypt</strong></a> объекта <strong>Енвелопеддата</strong> в объекте <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> не указан получатель. <br /> Чтобы добавить получателя, вызовите метод <a href="recipients-add.md"><strong>Recipients. Add</strong></a> .<br /> | 0x80880282 | 
| <strong>CAPICOM_E_ENVELOP_RECIPIENT_NOT_FOUND</strong> | Не удается найти получателя в объекте <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> . <br /> Как правило, это не происходит с объектом <a href="envelopeddata.md"><strong>енвелопеддата</strong></a> , созданным CAPICOM; Однако если объект <strong>енвелопеддата</strong> был создан сторонним продуктом, сертификат получателя может не включаться в структуру PKCS #7.<br /> | 0x80880283 | 
| <strong>CAPICOM_E_ENCRYPT_NOT_INITIALIZED</strong> | Объект <a href="encrypteddata.md"><strong>EncryptedData</strong></a> не инициализирован. <br /> Чтобы инициализировать объект <a href="encrypteddata.md"><strong>EncryptedData</strong></a> , необходимо либо задать свойство <a href="encrypteddata-content.md"><strong>Content</strong></a> , либо вызвать метод <a href="encrypteddata-decrypt.md"><strong>дешифровки</strong></a> .<br /> | 0x80880290 | 
| <strong>CAPICOM_E_ENCRYPT_INVALID_TYPE</strong> | Объект <a href="encrypteddata.md"><strong>EncryptedData</strong></a> имеет недопустимый тип. <br /> Обычно это означает, что данные повреждены.<br /> | 0x80880291 | 
| <strong>CAPICOM_E_ENCRYPT_NO_SECRET</strong> | Секрет объекта <a href="encrypteddata.md"><strong>EncryptedData</strong></a> не инициализирован. <br /> Чтобы инициализировать секрет объекта <a href="encrypteddata.md"><strong>EncryptedData</strong></a> , вызовите метод <a href="encrypteddata-setsecret.md"><strong>сетсекрет</strong></a> .<br /> | 0x80880292 | 
| <strong>CAPICOM_E_PRIVATE_KEY_NOT_INITIALIZED</strong> | Объект <a href="privatekey.md"><strong>PrivateKey</strong></a> не инициализирован.<br /> | 0x80880300//v 2.0 | 
| <strong>CAPICOM_E_PRIVATE_KEY_NOT_EXPORTABLE</strong> | Не удается экспортировать объект <a href="privatekey.md"><strong>PrivateKey</strong></a> .<br /> | 0x80880301//v 2.0 | 
| <strong>CAPICOM_E_ENCODE_NOT_INITIALIZED</strong> | Объект <a href="encodeddata.md"><strong>енкодеддата</strong></a> не инициализирован.<br /> | 0x80880320//v 2.0 | 
| <strong>CAPICOM_E_EXTENSION_NOT_INITIALIZED</strong> | Объект <a href="extension.md"><strong>расширения</strong></a> не инициализирован.<br /> | 0x80880330//v 2.0 | 
| <strong>CAPICOM_E_PROPERTY_NOT_INITIALIZED</strong> | Свойство <a href="extendedproperty-propid.md"><strong>PropID</strong></a> объекта <a href="extendedproperty.md"><strong>ExtendedProperty</strong></a> не инициализировано.<br /> | 0x80880340//v 2.0 | 
| <strong>CAPICOM_E_FIND_INVALID_TYPE</strong> | Параметр <em>FindType</em> метода <a href="certificates-find.md"><strong>Certificates. Find</strong></a> не является значением перечисления <a href="capicom-certificate-find-type.md"><strong>CAPICOM_CERTIFICATE_FIND_TYPE</strong></a> .<br /> | 0x80880350//v 2.0 | 
| <strong>CAPICOM_E_FIND_INVALID_PREDEFINED_POLICY</strong> | Указана недопустимая Предопределенная политика для операции поиска.<br /> | 0x80880351//v 2.0 | 
| <strong>CAPICOM_E_CODE_NOT_INITIALIZED</strong> | Объект <a href="signedcode.md"><strong>сигнедкоде</strong></a> не инициализирован.<br /> | 0x80880360//v 2.0 | 
| <strong>CAPICOM_E_CODE_NOT_SIGNED</strong> | Объект <a href="signedcode.md"><strong>сигнедкоде</strong></a> не подписан.<br /> Чтобы подписать объект <a href="signedcode.md"><strong>сигнедкоде</strong></a> , вызовите метод <a href="signedcode-sign.md"><strong>Sign</strong></a> .<br /> | 0x80880361//v 2.0 | 
| <strong>CAPICOM_E_CODE_DESCRIPTION_NOT_INITIALIZED</strong> | Свойство <a href="signedcode-description.md"><strong>Description</strong></a> объекта <a href="signedcode.md"><strong>сигнедкоде</strong></a> не инициализировано.<br /> | 0x80880362//v 2.0 | 
| <strong>CAPICOM_E_CODE_DESCRIPTION_URL_NOT_INITIALIZED</strong> | Свойство <a href="signedcode-descriptionurl.md"><strong>дескриптионурл</strong></a> объекта <a href="signedcode.md"><strong>сигнедкоде</strong></a> не инициализировано.<br /> | 0x80880363//v 2.0 | 
| <strong>CAPICOM_E_CODE_INVALID_TIMESTAMP_URL</strong> | Недопустимый параметр <em>URL-адреса</em> метода <a href="signedcode-timestamp.md"><strong>сигнедкоде. timestamp</strong></a> .<br /> | 0x80880364//v 2.0 | 
| <strong>CAPICOM_E_HASH_NO_DATA</strong> | Объект <a href="hasheddata.md"><strong>хашеддата</strong></a> не содержит данных.<br /> | 0x80880370//v 2.0 | 
| <strong>CAPICOM_E_INVALID_CONVERT_TYPE</strong> | Недопустимый тип преобразования.<br /> | 0x80880380//v 2.0 | 
| <strong>CAPICOM_E_NOT_SUPPORTED</strong> | Запрошенная операция не поддерживается на текущей платформе. <br /> | 0x80880900 | 
| <strong>CAPICOM_E_UI_DISABLED</strong> | При подписывании свойство <a href="signer-certificate.md"><strong>сертификата</strong></a> объекта <a href="signer.md"><strong>подписавши</strong></a> не было задано, но запрос сертификата пользователя был отключен. <br /> либо включите запрос, задавая свойство <a href="settings-enablepromptforcertificateui.md"><strong>енаблепромптфорцертификатеуи</strong></a> объекта <a href="settings.md"><strong>Параметры</strong></a> , либо задайте свойство <a href="signer-certificate.md"><strong>Certificate</strong></a> объекта <a href="signer.md"><strong>sign</strong></a> .<br /> | 0x80880901 | 
| <strong>CAPICOM_E_CANCELLED</strong> | Операция отменена пользователем. <br /> Это происходит, когда пользователю предлагается разрешение на выполнение определенной операции, например доступ к закрытому ключу, и пользователь отменяет операцию.<br /> | 0x80880902 | 
| <strong>CAPICOM_E_NOT_ALLOWED</strong> | Предпринятая операция не разрешена.<br /> Например, изменение свойства <a href="extendedproperty-propid.md"><strong>PropID</strong></a> объекта <a href="extendedproperty.md"><strong>ExtendedProperty</strong></a> не допускается, если объект присоединен к сертификату.<br /> | 0x80880903//v 2.0 | 
| <strong>CAPICOM_E_OUT_OF_RESOURCE</strong> | Элемент CAPICOM запустил ресурс.<br /> | 0x80880904//v 2.0 | 
| <strong>CAPICOM_E_INTERNAL</strong> | Произошла внутренняя ошибка. <br /> Обратитесь за помощью в службу технической поддержки Майкрософт.<br /> | 0x80880911 | 
| <strong>CAPICOM_E_UNKNOWN</strong> | Произошла неизвестная ошибка. <br /> Собирайте как можно больше информации и обратитесь к поставщику.<br /> | 0x80880999 | 




## <a name="requirements"></a>Требования



| Требование | Значение |
|----------------------------|--------------------------------------------------------------------------------------|
| Распространяемые компоненты<br/> | CAPICOM 2,0 или более поздней версии на Windows Server 2003 и Windows XP<br/>                |
| Заголовок<br/>          | <dl> <dt>CAPICOM. h</dt> </dl> |



 

 




