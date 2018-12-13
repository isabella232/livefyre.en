---
description: This method returns the URN for this network’s user.
seo-description: This method returns the URN for this network’s user.
seo-title: getUrnForUser Network Method
solution: Experience Manager
title: getUrnForUser Network Method
uuid: b70b8b0f-2b3a-4a1d-90d0-93a97a137ad4
index: y
internal: n
snippet: y
---

# getUrnForUser Network Method{#geturnforuser-network-method}

This method returns the URN for this network’s user.

<table id="properties_gq4_jyf_5y" class="simpletable properties" cellpadding="4" cellspacing="0"> 
 <thead class="prophead sthead"> 
  <th class="proptypehd"> Variable </th> 
  <th class="propvaluehd"> Type </th> 
  <th class="propdeschd"> Description </th> 
 </thead> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> userId </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> <p>The userId to use in the URN.</p> </td> 
 </tr> 
</table>

## Java Example {#section_nyl_ycs_rz}

```
network.getUrnForUser(userId);
```

Sample output:

```
"urn:livefyre:network=`example.fyre.co`:user=tester" 

```

## NodeJS Example {#section_xkd_gds_rz}

```
network.getUrnForUser(userId);
```

Sample output:

```
"urn:livefyre:network=`example.fyre.co`:user=tester" 

```

## PHP Example {#section_ghf_gds_rz}

```
$network->getUrnForUser(userId); 

```

Sample output:

```
"urn:livefyre:network=`example.fyre.co`:user=tester" 

```

## Python Example {#section_dwg_gds_rz}

```
network.get_urn_for_user(userId) 

```

Sample output:

```
"urn:livefyre:network=`example.fyre.co`:user=tester" 

```

## Ruby Example {#section_enh_gds_rz}

```
network.get_urn_for_user(userId) 

```

Sample output:

```
"urn:livefyre:network=`example.fyre.co`:user=tester" 

```

