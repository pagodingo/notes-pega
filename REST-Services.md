# REST Services

Exposing PEGA Data model(s) through REST Services:

**Activity-less** approach:

|Data Model||
|-|-|
|<u>Product</u>||
||ProductName|
||ProductPrice|
||ProductDescription|

|**Parent Class**|
|-|
|OOO-AAA-Int-|

|**(Parent Class): + Property**|Name|Type|Referenced Data Page|
|-|-|-|-|
||.GetAllProducts|Page List|D_ProductList

|**Service Package**|Name|Associated Class|
|-|-|-|
||RESTServicesPackage|****Parent Class****|

|REST Service|Name|Resource <span style="color: red">*</span>|Method|Request|Response <span style="color: red">*</span>|
|-|-|-|-|-|-|
|**Methods:**||||
||/GetAllProducts (app.pega.com/GetAllProducts)|**Parent Class**|GET||JSON, Map From Key: .GetAllProducts|

Defining your Service Package & Property in the root of your Application's Integration class may not always be ideal. You can optionally create a `OOO-AAA-Int-RESTServices` class to house your **Service Package**, **Response Properties**, and **Service(s)**.
