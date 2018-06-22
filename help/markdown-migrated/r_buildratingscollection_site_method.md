---
---

|  Variable  | Type  | Description  |
|---|---|---|
|  `varname  title`  | String  |
The title for the Collection.

|
|  `varname  articleId`  | String  | A unique article ID you chose to identify a Collection within your site.  |
|  `varname  url`  | String  | The canonical absolute URL for this Collection.  |
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
$collection = site-&gt;buildRatingsCollection(title, articleId, url); 

```
## Python Example {#section_dwg_gds_rz}

```
collection = site.build_ratings_collection(title, articleId, url) 

```
## Ruby Example {#section_enh_gds_rz}

```
collection = site.build_ratings_collection(title, articleId, url) 

```
