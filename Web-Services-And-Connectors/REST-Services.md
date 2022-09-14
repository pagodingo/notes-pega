# REST Services

Exposing PEGA Data model(s) through REST Services:

**Activity-less** approach:

---

**<u>Ingredients:</u>**

|**Parent Class**|
|-|
|OOO-AAA-Int-|

|Data Model||
|-|-|
|<u>Product</u>||
||ProductName|
||ProductPrice|
||ProductDescription|

|**Service Package**|Name|Associated Class|
|-|-|-|
||RESTServicesPackage|****Parent Class****|

|**(Parent Class): + Property**|Name|Type|Referenced Data Page|
|-|-|-|-|
||.GetAllProducts|Page List|D_ProductList



|REST Service|Name|Resource <span style="color: red">*</span>|Method|Request|Response <span style="color: red">*</span>|
|-|-|-|-|-|-|
|**Methods:**||||
||/GetAllProducts (app.pega.com/GetAllProducts)|**Parent Class**|GET||JSON, Map From Key: .GetAllProducts|

---

Defining your Service Package & Property in the root of your Application's Integration class may not always be ideal. You can optionally create a `OOO-AAA-Int-RESTServices` class to house your **Service Package**, **Response Properties**, and **Service(s)**.

It is not always clear that a REST service/connector will not be utilized by other apps internally. Therefore, generally it is a good rule of thumb to store authorization details in your application's enterprise (organization) layer.

**Walkthrough:**

<iframe src="https://drive.google.com/file/d/1RAY19vV5MncY4IUIEipih10dpE6E9OUK/preview" width="840" height="480" allow="autoplay"></iframe>