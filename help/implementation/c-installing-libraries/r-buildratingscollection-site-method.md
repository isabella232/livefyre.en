---
description: Returns a Collection object instantiated as a Ratings type. Run create_or_update() from the Collection object to complete the build process.
seo-description: Returns a Collection object instantiated as a Ratings type. Run create_or_update() from the Collection object to complete the build process.
seo-title: buildRatingsCollection Site Method
title: buildRatingsCollection Site Method
uuid: 5eea2ba3-48e1-4cd2-aa73-ea81788af1df
index: y
internal: n
snippet: y
---

# buildRatingsCollection Site Method{#buildratingscollection-site-method}

Returns a Collection object instantiated as a Ratings type. Run create_or_update() from the Collection object to complete the build process.

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
Collection collection = site.buildRatingsCollection(title, articleId, url); 

```

## NodeJS Example {#section_xkd_gds_rz}

```
var collection = site.buildRatingsCollection(title, articleId, url); 

```

## PHP Example {#section_ghf_gds_rz}

```
$collection = site->buildRatingsCollection(title, articleId, url); 

```

## Python Example {#section_dwg_gds_rz}

```
collection = site.build_ratings_collection(title, articleId, url) 

```

## Ruby Example {#section_enh_gds_rz}

```
collection = site.build_ratings_collection(title, articleId, url) 

```

