# Configuring REST Services

Exposing PEGA Data model(s) through REST Services:

**Activity-less** approach:

|Data Model|||
|-|-|-|
|Product|||
||ProductName||
||ProductPrice||
||ProductDescription||

|**Parent Class**||
|-|-|
|OOO-AAA-Int-||

|**Parent Class Property**|Name|Type|Referenced Data Page|
|-|-|-|-|
||.GetAllProducts|Page List|D_ProductList

|**Service Package**|Name|Associated Class||
|-|-|-|-|
||RESTServicesPackage|OOO-AAA-Int-||


|REST Service|Method|Request|Response||
|-|-|-|-|-|
|**Methods**|||||
||GET||JSON, Map From Key: .GetAllProducts||