---
description: Returns a Collection object instantiated as a Blog type. Run create_or_update() from the Collection object to complete the build process.
seo-description: Returns a Collection object instantiated as a Blog type. Run create_or_update() from the Collection object to complete the build process.
seo-title: buildBlogCollection Site Method
solution: Experience Manager
title: buildBlogCollection Site Method
uuid: 7dcdc74e-cb0f-4a64-ad47-883c3b1b894e
index: y
internal: n
snippet: y
translate: y
---

# buildBlogCollection Site Method


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
  <td class="propdesc stentry"> <p>A unique article ID you chose to identify a Collection within your site.</p> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> url </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> <p>The canonical absolute URL for this Collection.</p> </td> 
 </tr> 
</table>


## Java Example {#section_nyl_ycs_rz}


```
Collection collection = site.buildBlogCollection(title, articleId, url); 

```

## NodeJS Example {#section_xkd_gds_rz}


```
var collection = site.buildBlogCollection(title, articleId, url); 

```

## PHP Example {#section_ghf_gds_rz}


```
$collection = site->buildBlogCollection(title, articleId, url); 

```

## Python Example {#section_dwg_gds_rz}


```
collection = site.build_blog_collection(title, articleId, url) 

```

## Ruby Example {#section_enh_gds_rz}


```
collection = site.build_blog_collection(title, articleId, url) 

```
