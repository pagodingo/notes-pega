# Configuring REST Services

Exposing PEGA Data model(s) through REST Services:

**Activity-less** approach:

|Data Model||
|-|-|
|<u>Product</u>||
||ProductName|
||ProductPrice|
||ProductDescription|

Defining your Service Package & Property in the root of your Application's Integration class may not be desired. You can optionally create a `OOO-AAA-Int-RESTServices` class to house your **Service Package**, **Response Properties**, and **Services**.

|**Parent Class**|
|-|
|OOO-AAA-Int-|

|**Parent Class Property**|Name|Type|Referenced Data Page|
|-|-|-|-|
||.GetAllProducts|Page List|D_ProductList

|**Service Package**|Name|Associated Class|
|-|-|-|
||RESTServicesPackage|OOO-AAA-Int-|

|REST Service|Method|Request|Response|
|-|-|-|-|
|**Methods:**||||
||GET||JSON, Map From Key: .GetAllProducts|