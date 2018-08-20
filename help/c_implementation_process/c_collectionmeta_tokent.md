---
description: Create a unique token on your server that identifies every collection that you create.
seo-description: Create a unique token on your server that identifies every collection that you create.
seo-title: CollectionMeta Token
solution: Experience Manager
title: CollectionMeta Token
uuid: e70f95c6-de39-4cdd-9722-c86ef9916ffa
index: y
internal: n
snippet: y
translate: y
---

# CollectionMeta Token


<a id="section_ort_f4n_sz"></a>

Livefyre assigns a unique identifier to every Collection you create. Livefyre assigns a title, URL, and other parameters, including:

#### collectionMeta Token Parameters
<table frame="all" rowsep="1" colsep="1" id="table_ggl_gnn_sz">  
 <thead> 
  <tr> 
   <th class="entry"> Parameter </th> 
   <th class="entry"> Type </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> networkName </td> 
   <td> String (optional) </td> 
   <td> <p>The name of the Livefyre network (available from <span class="uicontrol"> Studio &amp;gt; Settings &amp;gt; Integration Settings &amp;gt; Credentials </span>). This is optional when using the library to create a collectionMeta token.</p> </td> 
  </tr> 
  <tr> 
   <td> networkKey </td> 
   <td> String (optional) </td> 
   <td> The secret key for the specific network (available from <span class="uicontrol"> Studio &amp;gt; Settings &amp;gt; Integration Settings &amp;gt; Credentials </span>). This is optional when using the library to create a collectionMeta token. </td> 
  </tr> 
  <tr> 
   <td> siteId </td> 
   <td> String (optional) </td> 
   <td> The ID for the site (available from <span class="uicontrol"> Studio &amp;gt; Settings &amp;gt; Integration Settings &amp;gt; Credentials </span>). Optional when using the library to create a collectionMeta token. </td> 
  </tr> 
  <tr> 
   <td> siteKey </td> 
   <td> String (optional) </td> 
   <td> The secret key for the site (available from <span class="uicontrol"> Studio &amp;gt; Settings &amp;gt; Integration Settings &amp;gt; Credentials </span>). </td> 
  </tr> 
  <tr> 
   <td> articleId </td> 
   <td> String (optional) </td> 
   <td> A unique ID for the Collection. </td> 
  </tr> 
  <tr> 
   <td> title </td> 
   <td> String (optional) </td> 
   <td> <p>The title you wish to apply to the Collection. Usually, this corresponds to the title of the page that displays the App.</p> <p>For example: “Integration is So Much Fun!”</p> <p>Note:  The max character length for the title is 255 characters. The title field does not support HTML entities. Please encode special characters using UTF-8. </p> </td> 
  </tr> 
  <tr> 
   <td> url </td> 
   <td> String (optional) </td> 
   <td> <p>The canonical absolute URL you wish to attach to this Collection. This URL will be used to generate links back to the App from content shared on Facebook and Twitter, email notifications, and Livefyre Studio.</p> <p>Note:  If testing locally, use a valid base URL domain (For example: <i><b>valid</b></i>: http://customer.com; <i><b>invalid</b></i>: http://localhost:5995). </p> </td> 
  </tr> 
  <tr> 
   <td> tags </td> 
   <td> String (optional) </td> 
   <td> <p>A comma-separated list of single keywords or phrases. Search Collections by tags using Studio. </p> <p>Note:  Tags cannot contain spaces. Use underscores if you wish a space to appear in the UI. </p> </td> 
  </tr> 
  <tr> 
   <td> extensions </td> 
   <td> JSON (optional) </td> 
   <td> A JSON-formatted set of params to pass along to the Collection. </td> 
  </tr> 
 </tbody> 
</table>


## Java {#section_orz_m4n_sz}


```
import com.livefyre.Livefyre; 
import com.livefyre.core.Network; 
import com.livefyre.core.Site; 
import com.livefyre.core.Collection; 
  
Network network = Livefyre.getNetwork("networkName", "networkKey"); 
Site site = network.getSite("siteId", "siteKey"); 
Collection collection = site.buildCommentsCollection("title", "articleId", "http://www.example.com"); 
collection.getData().setTags("tags"); 
  
String collectionMetaToken = collection.buildCollectionMetaToken(); 
 
 
```

## NodeJS {#section_kpk_44n_sz}


```
var livefyre = require('livefyre'); 
  
var network = livefyre.getNetwork('networkName', 'networkKey'); 
var site = network.getSite('siteId', 'siteKey'); 
var collection = site.buildCommentsCollection('title', 'articleId', 'http://www.example.com'); 
collection.data.tags = 'tags'; 
  
var collectionMetaToken = collection.buildCollectionMetaToken(); 

```

## PHP {#section_zmd_zbj_tz}


```
$network = Livefyre::getNetwork("networkName", "networkKey"); 
$site = $network->getSite("siteId", "siteKey"); 
$collection = $site->buildCommentsCollection("title", "articleId", "http://www.example.com"); 
$collection->getData()->setTags("tags"); 
  
$collectionMetaToken = $collection->buildCollectionMetaToken();
```

## Python {#section_rdm_prj_tz}


```
from livefyre import Livefyre 
  
network = Livefyre.get_network('networkName', 'networkKey') 
site = network.get_site('siteId', 'siteKey') 
collection = site.build_comments_collection('title', 'articleId', 'http://www.example.com') 
collection.data.tags = 'tags' 
  
collection_meta_token = collection.build_collection_meta_token()
```

## Ruby {#section_l5n_qrj_tz}


```
require 'livefyre' 
  
network = Livefyre.get_network('networkName', 'networkKey') 
site = network.get_site('siteId', 'siteKey') 
collection = site.build_comments_collection('title', 'articleId', 'http://www.example.com') 
collection.data.tags = 'tags' 
  
collection_meta_token = collection.build_collection_meta_token 

```

>[!NOTE] {importance="high"}
>
>Livefyre receives the collectionMeta token you build and determines uniqueness by combining siteId (Livefyre provided) and articleId (customer specified).

