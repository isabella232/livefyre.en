---
description: Create a checksum using the Livefyre libraries.
seo-description: Create a checksum using the Livefyre libraries.
seo-title: Creating a Checksum
title: Creating a Checksum
---

# Creating a Checksum

## Java {#section_pfr_lqj_tz}

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
## NodeJS {#section_hnx_jqj_tz}

```
var livefyre = require('livefyre'); 
 
var network = livefyre.getNetwork('networkName', 'networkKey'); 
var site = network.getSite('siteId', 'siteKey'); 
var collection = site.buildCommentsCollection('title', 'articleId', 'http://www.example.com'); 
collection.data.tags = 'tags'; 
 
var collectionMetaToken = collection.buildCollectionMetaToken();
```
## PHP {#section_kmt_3qj_tz}

```
$network = Livefyre::getNetwork("networkName", "networkKey"); 
$site = $network-&gt;getSite("siteId", "siteKey"); 
$collection = $site-&gt;buildCommentsCollection("title", "articleId", "http://www.example.com"); 
$collection-&gt;getData()-&gt;setTags("tags"); 
 
$collectionMetaToken = $collection-&gt;buildCollectionMetaToken(); 

```
## Python {#section_y55_gqj_tz}

```
from livefyre import Livefyre 
 
network = Livefyre.get_network('networkName', 'networkKey') 
site = network.get_site('siteId', 'siteKey') 
collection = site.build_comments_collection('title', 'articleId', 'http://www.example.com') 
collection.data.tags = 'tags' 
 
collection_meta_token = collection.build_collection_meta_token()
```
## Ruby {#section_a3y_ypj_tz}

```
require 'livefyre' 
 
network = Livefyre.get_network('networkName', 'networkKey') 
site = network.get_site('siteId', 'siteKey') 
collection = site.build_comments_collection('title', 'articleId', 'http://www.example.com') 
collection.data.tags = 'tags' 
 
collection_meta_token = collection.build_collection_meta_token 

```
