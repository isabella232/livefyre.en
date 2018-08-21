---
description: Returns a Collection object instantiated as a Sidenotes type. Run create_or_update() from the Collection object to complete the build process.
seo-description: Returns a Collection object instantiated as a Sidenotes type. Run create_or_update() from the Collection object to complete the build process.
seo-title: buildSitenotesCollection Site Method
solution: Experience Manager
title: buildSitenotesCollection Site Method
uuid: 3de34ecd-f9e7-4bbd-b966-aea49d3ab9c5
index: y
internal: n
snippet: y
translate: y
---

# buildSitenotesCollection Site Method


<table id="properties_gq4_jyf_5y" class="simpletable properties" cellpadding="4" cellspacing="0"> 
 <thead class="prophead sthead"> 
  <th class="proptypehd"> Variable </th> 
  <th class="propvaluehd"> Type </th> 
  <th class="propdeschd"> Description </th> 
 </thead> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> title </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> <p>The title for the Collection.</p> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> articleId </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> A unique article ID you chose to identify a Collection within your site. </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> url </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> The canonical absolute URL for this Collection. </td> 
 </tr> 
</table>


## Java Example {#section_nyl_ycs_rz}


```
Collection collection = site.buildSidenotesCollection(title, articleId, url); 

```

## NodeJS Example {#section_xkd_gds_rz}


```
var collection = site.buildSidenotesCollection(title, articleId, url); 

```

## PHP Example {#section_ghf_gds_rz}


```
$collection = site->buildSidenotesCollection(title, articleId, url); 

```

## Python Example {#section_dwg_gds_rz}


```
collection = site.build_sidenotes_collection(title, articleId, url) 

```

## Ruby Example {#section_enh_gds_rz}


```
collection = site.build_sidenotes_collection(title, articleId, url) 

```
