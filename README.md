# pro-contacto-practica
## EJERCICIO 2
Un servidor HTTP es una pieza de software que procesa una aplicación del lado del servidor y trabaja bajo el protocolo HTTP, de forma bidireccional o unidireccional, así como también sincrónicas/asincrónicas siguiendo una transacción cliente-servidor donde el cliente establece la conexión enviando una petición, para que luego el servidor procese la petición, devuelva la resuelva y por último el cliente pueda interpretarla.
--Dentro del protocolo HTTP existen distintos métodos de petición o también denominados verbos HTTP, los cuales especifican la acción que se desea llevar a cabo sobre un recurso determinado, los más comunes son:
-GET (para consultar un recurso)
-POST (para crear nuevos recursos)
-PATCH (para aplicar modificaciones parciales sobre un recurso)
-PUT (para sustituir un recurso)
-DELETE (para eliminar un recurso en específico)

--Dentro de una comunicación HTTP, el request hace referencia a la petición generada y enviada por parte del cliente hacia el servidor, la cual contiene distintos campos, uno de ellos el método HTTP. Por otro lado, response hace referencia a la respuesta por parte del servidor a esa petición, generada por el cliente y ya procesada.
Los headers o cabeceras en una comunicación HTTP son encabezados que nos permiten agregar información adicional a la petición o respuesta, de manera de quedar personalizada de acuerdo a distintos criterios.

--Un Query string en el contexto de una URL, es básicamente todo lo que vemos en una URL luego del signo de pregunta, donde tenemos como parámetro un par key-value, teniendo en cuenta que podemos tener un solo parámetro o una combinación de parámetros concatenados con el signo ampersand (&)

--El responseCode, bajo el contexto de una comunicación HTTP, es el código de estado de la respuesta HTTP que indica de que manera se completó una solicitud específica. Estos códigos pueden variar según el contexto y los posibles valores devueltos pueden indicar una respuesta informativa, satisfactoria, de redirección, de errores de el/ los cliente/s o de errores de el/los servidor/es.


--La data en un GET se envía usando la URL,en el encabezado de la solicitud, llevando los datos de forma 'visible' al cliente, mientras que la data en un POST se envía en el cuerpo de la solicitud, de forma aparentemente 'oculta' de manera que no son visibles al usuario de la web.
-- El verbo http que utilizar el navegador para acceder a una página es GET

--La estructura XML es un lenguaje estándar de marcado, basado en el uso de etiquetas que se utilizan para el intercambio de información y para identificar los distintos componentes, junto con sus etiquetas y atributos. Un ejemplo de XML aplicado a Salesforce, es el siguiente 'package.xml manifest' que contiene distintos componentes metadatos y se los identifica para poder luego por ejemplo gestionar un deploy o un retrieve de unos pocos metadatos seleccionados de manera corta y rápida.

<?xml version="1.0" encoding="UTF-8"?>
<Package xmlns="http://soap.sforce.com/2006/04/metadata">
    <types>
        <members>CUSTOM OBJECT API NAME HERE</members>
        <name>CustomObject</name>
    </types>
    <types>
        <members>CUSTOM TAB API NAME HERE</members>
        <name>CustomTab</name>
    </types>
    <version>51.0</version>
</Package>

Luego, la estructura JSON es un formato de texto de fácil lectura y escritura, que sirve para representar datos estructurados en la sintaxis de objetos, que nos permite construir a su vez una jerarquía de datos y se utiliza generalmente al transmitir datos en aplicaciones web. Un ejemplo del mismo es el siguiente:
{
    "errors": [ "Data failed validation rules" ],
    "message": "Please edit and retry",
    "details": {
        "record": "001000000000001",
        "record_type": "Account"
    }
}

-- SOAP es un protocolo estándar para el diseño y construcción de servicios web que permite establecer comunicación entre sistemas a través de mensajes en HTTP y está basado en XML

--REST Full es un estilo de arquitectura para el desarrollo de aplicaciones donde el mecanismo de comunicación entre sistemas se establece a través de peticiones HTTP, utilizando para el intercambio de información: XML, JSON, entre otros.

--Los headers en un request son parte relevante de los HTTP request y transmiten información valiosa sobre la página solicitada, el servidor, el método HTTP,URL,versión, entre otros. El key Content-type en un header se usa para indicar el tipo de contenido original del recurso enviado, algunos de los mas conocidos son : application/json; application/xml; image/jpeg; text/html.

## EJERCICIO 3
-- La diferencia observada entre la llamada en el punto 1 y el punto 3 es que en ésta última, ya se encuentra ubicado el nombre y email que introducimos con la POST Request en el punto 2, de manera que se pueden visualizar los datos de Luca, en este caso.

## EJERCICIO 4
https://trailblazer.me/id/lucapero

## EJERCICIO 5
Las relaciones se adjuntan al final del ejercicio
1.Lead
El lead es un cliente potencial que tiene interés en un producto determinado o servicio el cual es ofrecido por la organización, de mucha importancia en las distintas estrategias de marketing. Disponen de información relacionada al interés del usuario, información de contacto, y preferencias de consumo.

Campos:
Address
AnnualRevenue
City
Company
ConvertedAccountId
ConvertedContactId
ConvertedDate
ConvertedOpportunityId
Country
CreatedById
CreatedDate
Description
Email
EmailBouncedDate
EmailBouncedReason
FirstName
GeocodeAccuracy
HasOptedOutOfEmail
HasOptedOutOfFax
Id
IndividualId
Industry
IsConverted
IsDeleted
IsUnreadByOwner
Jigsaw
JigsawContactId
LastActivityDate
LastModifiedById
LastModifiedDate
LastName
LastReferencedDate
LastViewedDate
Latitude
LeadSource
Longitude
MasterRecordId
Name
NumberOfEmployees
OwnerId
Phone
PhotoUrl
PostalCode
Rating
Salutation
State
Status
Street
SystemModstamp
Title
Website


2.Account
Account hace referencia a una cuenta individual, la cual puede representarse como una organización o una persona del negocio relacionado.
Los datos que almacenan son relacionados a la persona o el negocio, como la competencia,clientes,etc.
Campos:
AccountSource
AnnualRevenue
BillingAddress
BillingCity
BillingCountry
BillingGeocodeAccuracy
BillingLatitude
BillingLongitude
BillingPostalCode
BillingState
BillingStreet
CreatedById
CreatedDate
Description
Fax
Id
Industry
IsDeleted
Jigsaw
JigsawCompanyId
LastActivityDate
LastModifiedById
LastModifiedDate
LastReferencedDate
LastViewedDate
MasterRecordId
Name
NumberOfEmployees
OwnerId
ParentId
Phone
PhotoUrl
ShippingAddress
ShippingCity
ShippingCountry
ShippingGeocodeAccuracy
ShippingLatitude
ShippingLongitude
ShippingPostalCode
ShippingState
ShippingStreet
SicDesc
SystemModstamp
Type
Website


3.Contact
El objeto Contact representa un contacto, en otras palabras, una persona asociada a una cuenta. Este objeto almacena informacion individual del mismo, como por ejemplo Teléfono,emails, que pueden estar asociados a la cuenta.

Campos:
AccountId
AssistantName
AssistantPhone
Birthdate
CreatedById
CreatedDate
Department
Description
Email
EmailBouncedDate
EmailBouncedReason
Fax
FirstName
HasOptedOutOfEmail
HasOptedOutOfFax
HomePhone
Id
IndividualId
IsDeleted
IsEmailBounced
Jigsaw
JigsawContactId
LastActivityDate
LastCURequestDate
LastCUUpdateDate
LastModifiedById
LastModifiedDate
LastName
LastReferencedDate
LastViewedDate
LeadSource
MailingAddress
MailingCity
MailingCountry
MailingGeocodeAccuracy
MailingLatitude
MailingLongitude
MailingPostalCode
MailingState
MailingStreet
MasterRecordId
MobilePhone
Name
OtherAddress
OtherCity
OtherCountry
OtherGeocodeAccuracy
OtherLatitude
OtherLongitude
OtherPhone
OtherPostalCode
OtherState
OtherStreet
OwnerId
Phone
PhotoUrl
ReportsToId
Salutation
SystemModstamp
Title


4.Opportunity
El objeto Opportunity representa una oportunidad que puede considerarse como venta o posible negociación, éste almacena datos del proceso de negociación relacionado al intento de cierre de una venta a un cliente potencial.
Campos:
AccountId
Amount
CampaignId
CloseDate
ContactId
CreatedById
CreatedDate
Description
Fiscal
FiscalQuarter
FiscalYear
ForecastCategory
ForecastCategoryName
HasOpenActivity
HasOpportunityLineItem
HasOverdueTask
Id
IsClosed
IsDeleted
IsWon
LastActivityDate
LastAmountChangedHistoryId
LastCloseDateChangedHistoryId
LastModifiedById
LastModifiedDate
LastReferencedDate
LastStageChangeDate
LastViewedDate
LeadSource
Name
NextStep
OwnerId
Pricebook2Id
Probability
PushCount
StageName
SystemModstamp
Type


5.Product
El objeto Product representa un producto en específico que la empresa vende, y almacena datos relacionados a precios,cantidad,ingresos,etc.

Campos:
BillingPolicyId
CanUseQuantitySchedule
CanUseRevenueSchedule
ConnectionReceivedId
ConnectionSentId
CurrencyIsoCode
Description
DisplayUrl
ExternalDataSourceId
ExternalId
Family
IsActive
IsArchived
IsDeleted
LastReferencedDate
LastViewedDate
Name
NumberOfQuantityInstallments
NumberOfRevenueInstallments
ProductClass
ProductCode
QuantityInstallmentPeriod
QuantityScheduleType
QuantityUnitOfMeasure
RecalculateTotalPrice
RevenueInstallmentPeriod
RevenueScheduleType
StockKeepingUnit
Type
TaxPolicyId


6.PriceBook
El objeto PriceBook, hace referencia a un libro de precios el cual puede vincularse con el objeto Product, y proporciona una lista de productos y sus precios por unidad.

Campos:
CreatedById
CreatedDate
Description
Id
IsActive
IsArchived
IsDeleted
IsStandard
LastModifiedById
LastModifiedDate
LastReferencedDate
LastViewedDate
Name
SystemModstamp



7.Quote
El objeto Quote representa una cotización, almacena información relacionada a precios de productos y servicios,pueden vincularse con oportunidades y nos permite mostrar distintos tipos de combinaciones en cuanto a productos,descuentos y cantidades.

Campos:
AccountId
AdditionalAddress
AdditionalCity
AdditionalCountry
AdditionalCountryCode
AdditionalLatitude
AdditionalLongitude
AdditionalName
AdditionalPostalCode
AdditionalState
AdditionalStateCode
AdditionalStreet
BillingAddress
BillingCity
BillingCountry
BillingCountryCode
BillingLatitud
BillingLongitude
BillingName
BillingPostalCode
BillingState
BillingStateCode
BillingStreet
CalculationStatus
CanCreateQuoteLineItems
ContactId
ContractId
CurrencyIsoCode
Description
Discount
Email
ExpirationDate
Fax
GrandTotal
IsSyncing
LastReferencedDate
LastViewedDate
LineItemCount
Name
OpportunityId
Phone
Pricebook2Id
QuoteNumber
QuoteToAddress
QuoteToCity
QuoteToCountry
QuoteToLatitude
QuoteToLongitude
QuoteToName
QuoteToPostalCode
QuoteToState
QuoteToStreet
RecordTypeID
ShippingAddress
ShippingCity
ShippingCountry
ShippingCountryCode
ShippingHandling
ShippingLatitude
ShippingLongitude
ShippingName
ShippingPostalCode
ShippingState
ShippingStateCode
ShippingStreet
Status
Subtotal
Tax
TotalPrice
TotalPriceWithTax
TotalTaxAmount


8:Asset
El objeto Asset representa un producto de valor comercial vendido por la organización hacia un cliente. Almacena información relacionada a el producto vendido al cliente, de manera que se pueda hacer un seguimiento de estos.

Campos:
AccountId
AssetLevel
AssetProvidedById
AssetServicedById
Availability
AverageUptimePerDay
ConsequenceOfFailure
ContactId
CurrentAmount
CurrentLifecycleEndDate
CurrentMrr
CurrentQuantity
Description
DigitalAssetStatus
ExternalIdentifier
HasLifecycleManagement
InstallDate
IsCompetitorProduct
IsInternal
LastReferencedDate
LastViewedDate
LifecycleEndDate
LifecycleStartDate
LocationId
ManufactureDate
Name
OwnerId
ParentId
Price
Product2Id
ProductCode
ProductDescription
ProductFamily
PurchaseDate
Quantity
Reliability
RenewalTerm
RenewalTermUnit
RootAssetId
SerialNumber
Status
StatusReason
StockKeepingUnit
SumDowntime
SumUnplannedDowntime
TotalLifecycleAmount
UptimeRecordEnd
UptimeRecordStart
UsageEndDate
Uuid


9:Case
El objeto Case representa un caso tal como problema o queja del client. Este objeto se utiliza para poder gestionar los casos de la organización, y almacena información relacionada a los casos del cliente, asi como archivos adjuntos.

Campos:
AccountId
BusinessHoursId
Comments
CaseNumber
ClosedDate
CommunityId
ConnectionReceivedId
ConnectionSentId
ContactEmail
ContactFax
ContactId
ContactMobile
ContactPhone
CreatorFullPhotoUrl
CreatorName
CreatorSmallPhotoUrl
Description
FeedItemId
HasCommentsUnreadByOwner
HasSelfServiceComments
IsClosed
IsClosedOnCreate
IsDeleted
IsEscalated
IsSelfServiceClosed
IsStopped
IsVisibleInSelfService
Language
LastReferencedDate
LastViewedDate
MasterRecordId
Origin
OwnerId
ParentId
Priority
QuestionId
Reason
RecordTypeId
SlaStartDate
SourceId
Status
StopStartDate
Subject
SuppliedCompany
SuppliedEmail
SuppliedName
SuppliedPhone
Type


10:Article
El objeto Article almacena informacion acerca de los productos y servicios de la organización, luego podiendo clasificarlos en base a distintas categorias.

Campos:

ArchivedById
ArchivedDate
ArticleNumber
CaseAssociationCount
CreatedById
CreatedDate
DraftVersionId
FirstPublishedDate
Id
IsDeleted
LastArchivedVersionId
LastModifiedById
LastModifiedDate
LastPublishedDate
LastReferencedDate
LastViewedDate
MasterLanguage
MigratedToFromArticle
OnlineVersionId
SecurityId
SystemModstamp
TaskOwnerId
Title
TotalViewCount

## EJERCICIO 6
SOLUCIONES DE SALESFORCE
A. Salesforce es un CRM(Customer Relationship Management) personalizable que cuenta con distintas cloud para brindar a las empresas y clientes como solución para la gestión de relaciones con los clientes, en pocas palabras, es una plataforma integrada basada en la nube.

B. Sales Cloud
Sales Cloud es un módulo de la nube de Salesforce que se enfoca principalmente en las ventas, donde se puede hacer un seguimiento de las mismas de una manera detallada, gestionando de forma eficiente la relación con los clientes y la colaboración entre los equipos comerciales.
C. Service Cloud
Service Cloud es un módulo de la nube de Salesforce que se enfoca principalmente en toda la actividad relacionada con la atención al cliente, es una plataforma multicanal y otorga al cliente una atención individual y personalizada a sus necesidades.
D. Health Cloud
Health Cloud es un módulo de la nube de Salesforce que está enfocada principalmente en la gestión clínica de pacientes por medio de tecnologías on-cloud, ofreciendo una comunicación mas personalizada entre pacientes, y el resto del equipo en cualquier dispositivo.
E. Marketing Cloud
Marketing Cloud es un módulo de la nube de Salesforce que se enfoca principalmente en brindar distintas herramientas diseñadas que permiten gestionar de una manera eficiente la interacción de la marca con sus clientes, a través de diferentes canales. Es una plataforma que permite aumentar la captación de clientes y las ventas.
FUNCIONALIDADES DE SALESFORCE
A.	Un RecordType es, como lo indica la palabra, un tipo de registro que en SF nos permite definir los distintos niveles de información que se mostraran para cada uno de los perfiles de usuario.
B.	Un ReportType es un tipo de reporte en SF donde podemos definir una colección de objetos de Salesforce que queremos reportar de manera personalizable.
C.	Un Page Layout es una personalización que podemos definir en SF donde se controla la visibilidad de los botones, campos, links, related list,etc. en las Record Pages de los objetos.
D.	Un Compact Layout  muestra los campos clave de un registro de manera que se pueda visualizar lo más importante del mismo de forma inmediata.
E.	Un Perfil define como acceden los distintos usuarios a los objetos y datos que existen en SF y también los distintos accesos dentro de la aplicación.
F.	Un Rol permite determinar los niveles de visibilidad que un usuario tiene sobre los datos de su organización.
G.	Una Validation Rule es una herramienta que SF nos ofrece para poder definir reglas que se aplican en los distintos objetos con el fin de garantizar un correcto flujo del proceso de negocio.
H.	Existen varias diferencias en cuanto a una relación Master Detail y una relación Lookup, principalmente, la relación Master Detail es más fuerte que una Lookup ya que en la primera los objetos generan una dependencia de forma tal que cuando sea eliminado el registro padre, por consecuente los del hijo también, generando un borrado en “cascada”. Esto no ocurre así en Lookup, ya que es una relación más independiente.}
I.	Un Sandbox es una copia de la organización en un entorno aislado de producción, que se puede usar tanto como ambiente de prueba, como de desarrollo.
J.	Un ChangeSet es un paquete que nos permite enviar un conjunto de cambios (tanto de código como de metadatos personalizados a través de herramientas declarativas) desde una organización de SF a otra, siempre y cuando estén vinculadas.
K.	El Data Import Wizard de SF sirve para importar datos principalmente de varios objetos standards y custom de Salesforce con un límite de 50000 registros a la vez.
L.	La funcionalidad Web to Lead sirve para capturar información del cliente desde la web de manera tal que se puedan generar como nuevos Leads en Salesforce.
M.	La funcionalidad Web To Case sirve para recopilar solicitudes de servicio de atención al cliente directamente del sitio web de su compañía y que se puedan generar automáticamente como casos nuevos en Salesforce.
N.	La funcionalidad Omnichannel sirve para ofrecer una experiencia distinta mediante varios puntos de contacto de forma eficiente y teniendo en cuenta la prioridad de los elementos de trabajo.
O.	La funcionalidad Chatter sirve para que los usuarios puedan trabajar juntos, comunicarse y compartir información de manera inmediata, conectando y motivándolos a trabajar de una forma eficiente independientemente de la función o ubicación.
CONCEPTOS GENERALES.
A.	SaaS significa Software As A Service, consiste en alojar soporte informático y datos en Internet para que pueda ser usado por aquellas empresas que contratan el servicio, sin tener que instalar programas en sus ordenadores y otros equipos informáticos.
B.	Salesforce es Saas ya que se puede acceder al software en cualquier momento, desde cualquier dispositivo que tenga conexión a Internet y desde el navegador, permitiendo contratar distintas licencias para el caso en específico.
C.	Que una solución sea Cloud quiere decir que entrega o vende los servicios informáticos on-demand a través de Internet, de una forma muy accesible y fácil, preparado para las necesidades particulares del cliente.
D.	Que una solución sea On-Premise quiere decir que el software se instala y ejecuta en los equipamientos de la persona u organización que usará el software, es decir, en los equipos físicos, y no a través de Internet.
E.	Un pipeline de ventas es el proceso de actividades y estrategias que necesita un vendedor para acelerar el ciclo de ventas, transformando clientes potenciales en clientes finales.
F.	El funnel de ventas es un sistema o representación gráfica diseñado para atraer a usuarios, convertirlos en leads y transformarlos en clientes finales.
G.	 Customer Experience es un término que hace referencia las estrategias que las empresas utilizan para que la experiencia de los clientes sea lo mejor posible durante todo el proceso involucrado. Es la experiencia que formará el cliente en función de las interacciones con la marca de la empresa.
H.	Omnicanalidad es un término que hace referencia a una estrategia de comunicación orientada a la atención al cliente, de manera que se disponga de un sistema omnicanal para poder ofrecer múltiples medios de atención para garantizar una experiencia del usuario satoisfactoria, se la puede ligar con el objetivo de Customer Experience.
I.	Un negocio B2B (Business to Business) es aquel que tiene como objetivo principal las ventas de una empresa a otra, donde los clientes son empresas que representan sectores específicos del mercado. Es un negocio donde se forjan relaciones duraderas con cada cliente.
Por otro lado, un negocio B2C(Business to Customer) es aquel cuyo modelo de negocio se basa en la venta hacia un consumidor final, es el modelo de las empresas que ofrecen bienes y servicios de consumo masivo , donde el proceso para cerrar una venta es rápido.
KPI es un término (Key Performance Indicator), cuyo significado representa indicador clave de desempeño, y hace referencia a un conjunto de valores, métricas que un negocio establece para sintetizar la información sobre la eficacia y productividad, y de esta manera determinar el éxito o no.
J.	Una API (Application Programming Interface) es una interfaz de programación de aplicaciones que permite la interacción y comunicación entre sistemas informáticos, bajo un conjunto de reglas y protocolos preestablecidas que se utilizan para diseñar e integrar el software de las aplicaciones.
Una REST API es una API que se ajusta a los principios de diseño REST, un estilo de arquitectura que permite a una aplicación o servicio acceder a un recurso dentro de otra aplicación o servicio. Dispone de tres recurso principales: Cliente, Servidor y Recursos.
K.	Un proceso Batch es aquel que ejecuta una serie de operaciones sin la necesidad de una supervisión directa del usuario; en SF es una herramienta asíncrona que nos permite operar con registros de forma masiva, en comparación a las herramientas síncronas,  debido a la extensión de los limites normales, y es usada principalmente para la actualización o borrado masivo de registros.
L.	Kanban es un término que hace referencia a una metodología de trabajo que se basa en el tablero Kanban, que nos permite representar la producción, y demanda de los clientes de forma tal de poder gestionar el trabajo pudiendo visualizar donde existiesen cuellos de botella o alguna interrupción en el flujo de trabajo, con el objetivo de ayudar al equipo a encontrar un equilibrio entre el trabajo que deben hacer y la disponibilidad de cada miembro del equipo.
M.	Un ERP es un sistema de software que ayuda a gestionar todo el negocio de una empresa, incluyendo procesos de finanzas, recursos humanos, fabricación, etc. que brinda la integración para ejecutar todas las operaciones diarias del negocio.
N.	Salesforce no es un ERP, es más bien un CRM, ya que ofrece variadas soluciones de negocio, que pueden ser integradas y dar soporte a un sistema ERP, pero no provee un producto ERP completo, si bien mejora la eficiencia de las operaciones, tienen distintos propósitos, aunque pueden utilizarse de manera complementaria para abarcar todos los aspectos del negocio.

## EJERCICIO 7
