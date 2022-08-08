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

**Walkthrough:**

<iframe src="https://drive.google.com/file/d/1RAY19vV5MncY4IUIEipih10dpE6E9OUK/preview" width="840" height="480" allow="autoplay"></iframe>

<video tabindex="-1" id="vjs_video_912_html5_api" data-player="obdhcLv77W" data-account="1519050010001" data-video-id="6254871655001" data-media-duration="" data-playback-rates="[.75, 1, 1.25, 1.5, 2]" data-application-id="" data-embed="default" class="vjs-tech" data-pega-video-asset-type="Video" data-pega-video-type="Video" data-src="https://players.brightcove.net/1519050010001/obdhcLv77W_default/index.html?videoId=6254871655001" preload="metadata" poster="https://cf-images.us-east-1.prod.boltdns.net/v1/static/1519050010001/388abf2b-4afa-4c5e-8ccf-c7c4d715ec0e/9d72bb29-d18b-4eed-a6c0-77a39ff995c6/1280x720/match/image.jpg" src="blob:https://academy.pega.com/4a656705-1af9-4176-a036-02b19fb0830c"></video>