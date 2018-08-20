---
description: Returns an encrypted user authenticated token for the network it is called from.
seo-description: Returns an encrypted user authenticated token for the network it is called from.
seo-title: buildUserAuthToken Network Method
solution: Experience Manager
title: buildUserAuthToken Network Method
uuid: 141ce3a7-11fb-48bf-b2a1-58abdd8df9c6
index: y
internal: n
snippet: y
translate: y
---

# buildUserAuthToken Network Method


<table id="properties_gq4_jyf_5y" class="simpletable properties" cellpadding="4" cellspacing="0"> 
 <thead class="prophead sthead"> 
  <th class="proptypehd"> Variable </th> 
  <th class="propvaluehd"> Type </th> 
  <th class="propdeschd"> Description </th> 
 </thead> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> userId </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> <p>The user ID for the user to whom this token belongs.</p> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> displayName </span> </td> 
  <td class="propvalue stentry"> String </td> 
  <td class="propdesc stentry"> The display name for the user. </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry"> <span class="varname"> expires </span> </td> 
  <td class="propvalue stentry"> Double </td> 
  <td class="propdesc stentry"> When the token should expire in seconds. </td> 
 </tr> 
</table>


## Java Example {#section_nyl_ycs_rz}


```
network.buildUserAuthToken(userId, displayName, expires); 

```
Sample output: 

```
eyJhbGciOiJIUzI1NiJ9.eyJkb21haW4iOiJ0ZXN0LmZ5cmUuY29tIiwidXNlcl9pZCI6InN5c3RlbSIsImRpc3BsYXlfbmFtZSI6InN5c3RlbSIsImV4cGlyZXMiOjEzOTY2NTUwODN9.33GuJF_ou2O6CCV22Y3PlLUgP2Igy9vAXfmLONkt-Yo 

```

## NodeJS Example {#section_xkd_gds_rz}


```
network.buildUserAuthToken(userId, displayName, expires); 

```
Sample output: 

```
eyJhbGciOiJIUzI1NiJ9.eyJkb21haW4iOiJ0ZXN0LmZ5cmUuY29tIiwidXNlcl9pZCI6InN5c3RlbSIsImRpc3BsYXlfbmFtZSI6InN5c3RlbSIsImV4cGlyZXMiOjEzOTY2NTUwODN9.33GuJF_ou2O6CCV22Y3PlLUgP2Igy9vAXfmLONkt-Yo 

```

## PHP Example {#section_ghf_gds_rz}


```
$network->buildUserAuthToken(userId, displayName, expires); 

```
Sample output: 

```
eyJhbGciOiJIUzI1NiJ9.eyJkb21haW4iOiJ0ZXN0LmZ5cmUuY29tIiwidXNlcl9pZCI6InN5c3RlbSIsImRpc3BsYXlfbmFtZSI6InN5c3RlbSIsImV4cGlyZXMiOjEzOTY2NTUwODN9.33GuJF_ou2O6CCV22Y3PlLUgP2Igy9vAXfmLONkt-Yo
```

## Python Example {#section_dwg_gds_rz}


```
network.build_user_auth_token(userId, displayName, expires) 

```
Sample output: 

```
eyJhbGciOiJIUzI1NiJ9.eyJkb21haW4iOiJ0ZXN0LmZ5cmUuY29tIiwidXNlcl9pZCI6InN5c3RlbSIsImRpc3BsYXlfbmFtZSI6InN5c3RlbSIsImV4cGlyZXMiOjEzOTY2NTUwODN9.33GuJF_ou2O6CCV22Y3PlLUgP2Igy9vAXfmLONkt-Yo
```

## Ruby Example {#section_enh_gds_rz}


```
network.build_user_auth_token(userId, displayName, expires) 

```
Sample output: 

```
eyJhbGciOiJIUzI1NiJ9.eyJkb21haW4iOiJ0ZXN0LmZ5cmUuY29tIiwidXNlcl9pZCI6InN5c3RlbSIsImRpc3BsYXlfbmFtZSI6InN5c3RlbSIsImV4cGlyZXMiOjEzOTY2NTUwODN9.33GuJF_ou2O6CCV22Y3PlLUgP2Igy9vAXfmLONkt-Yo
```
