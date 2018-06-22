---
description: Count the number of curated social items.
seo-description: Count the number of curated social items.
seo-title: Social Counter
solution: Experience Manager
title: Social Counter
---

# Social Counter

For a complete list of available endpoints, please see the Livefyre [ API Reference ](http://livefyre-devhub-production.herokuapp.com/developers/api-reference/) section.

The Social Counter API returns counts for matched curation rules in a given collection for intervals over a period of time.

>[!NOTE]
>
>This API is available only for Twitter hashtags.
Social Counter API:

* Resource
* Rule Types
* Response
## Resource {#section_p2s_2hc_11b}

```
GET https://{networkName}.bootstrap.fyre.co/api/v3.0/stats.collections.curate/{query}.json
```
<table id="table_tvt_l2l_wz"> 
 <title>Relative Time</title> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Abbreviation </th> 
    <th class="entry"> Unit </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> s </td> 
    <td> Seconds </td> 
   </tr> 
   <tr> 
    <td> min </td> 
    <td> Minutes </td> 
   </tr> 
   <tr> 
    <td> h </td> 
    <td> Hours </td> 
   </tr> 
   <tr> 
    <td> d </td> 
    <td> Days </td> 
   </tr> 
   <tr> 
    <td> w </td> 
    <td> Weeks </td> 
   </tr> 
   <tr> 
    <td> mon </td> 
    <td> 30 Days (Month) </td> 
   </tr> 
   <tr> 
    <td> y </td> 
    <td> 365 Days (Year) </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

Example:

```
https://labs-t402.bootstrap.fyre.co/api/v3.0/stats.collections.curate/MTIzNDU2OnNvbWUtYXJ0aWNsZS1pZDsy.json&amp;from=-7d&amp;until=-6d
```
## Absolute Time {#section_xqr_jgc_11b}

FORMAT: HH:MM_YYYYMMDD

<table id="table_vvt_l2l_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Abbreviation </th> 
    <th class="entry"> Meaning </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> HH </td> 
    <td> Hours (in 24h clock format) </td> 
   </tr> 
   <tr> 
    <td> MM </td> 
    <td> Minutes </td> 
   </tr> 
   <tr> 
    <td> YYYY </td> 
    <td> 4-Digit Year </td> 
   </tr> 
   <tr> 
    <td> MM </td> 
    <td> Month </td> 
   </tr> 
   <tr> 
    <td> DD </td> 
    <td> Day </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

Example:

```
https://labs-t402.bootstrap.fyre.co/api/v3.0/stats.collections.curate/MTIzNDU2OnNvbWUtYXJ0aWNsZS1pZDsy.json&amp;from=04:00_20130709 

```
## Rule Types {#section_v53_xqb_11b}

<table id="table_xvt_l2l_wz"> 
 <tgroup cols="2"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <thead> 
   <tr> 
    <th class="entry"> Value </th> 
    <th class="entry"> Type </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> 2 </td> 
    <td> Twitter </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

Example:

To obtain counts over the last minute for site “123456” and article ID “some-article-id” and rule-type “2”, for example: 123456:some-article-id;2:

```
curl -XGET "https://labs-t402.bootstrap.fyre.co/api/v3.0/stats.collections.curate/MTIzNDU2OnNvbWUtYXJ0aWNsZS1pZDsy.json&amp;from=-1min" 

```
Example Response:

```
{ 
 "status": "ok", 
 "code": 200, 
 "data": { 
 "123456": { 
 "some-article-id": { 
 "2": [ 
 [ 
 2, 
 1374770460 
 ], 
 [ 
 4, 
 1374770470 
 ], 
 [ 
 3, 
 1374770480 
 ], 
 [ 
 1, 
 1374770490 
 ], 
 [ 
 0, 
 1374770500 
 ], 
 [ 
 7, 
 1374770510 
 ] 
 ] 
 } 
 } 
 } 
}
```
