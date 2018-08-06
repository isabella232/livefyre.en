---
description: Returns a new Site object.
seo-description: Returns a new Site object.
seo-title: getSite Network Method
solution: Experience Manager
title: getSite Network Method
uuid: 3cebf97b-3fba-42f8-a120-a9f0269c0d4f
index: y
internal: n
snippet: y
translate: y
---

# getSite Network Method


|  * ` siteId` * | String  | The Livefyre-provided ID for the website or application to which the Collection belongs. For example: 303617.  |
|---|---|---|
|  * ` siteKey` * | String  | The Livefyre-provided secret key for siteId.  |


## Java Example {#section_nyl_ycs_rz}


```
Site site = network.getSite(siteId, siteKey); 

```

## NodeJS Example {#section_xkd_gds_rz}


```
var site = network.getSite(siteId, siteKey); 

```

## PHP Example {#section_ghf_gds_rz}


```
$site = $network->getSite(siteId, siteKey); 
 

```

## Python Example {#section_dwg_gds_rz}


```
site = network.get_site(siteId, siteKey) 

```

## Ruby Example {#section_enh_gds_rz}


```
site = network.get_site(siteId, siteKey) 

```
