---
description: Informs Livefyre to update the network’s user sync URL to the one provided. Returns a Boolean.
seo-description: Informs Livefyre to update the network’s user sync URL to the one provided. Returns a Boolean.
seo-title: setUserSyncUrl Network Method
solution: Experience Manager
title: setUserSyncUrl Network Method
uuid: c1321e47-199c-4d83-a8b3-8096d805e754
index: y
internal: n
snippet: y
translate: y
---

# setUserSyncUrl Network Method


|  *` urlTemplate`* | String  | The URL to register with Livefyre for syncing user IDs. Requires “{id}” to be part of the provided URL string  |
|---|---|---|


## Java Example {#section_nyl_ycs_rz}


```
network.setUserSyncUrl(urlTemplate); 

```
Sample output: 

```
true
```

## NodeJS Example {#section_xkd_gds_rz}


```
network.setUserSyncUrl(urlTemplate); 

```
Sample output: 

```
true
```

## PHP Example {#section_ghf_gds_rz}


```
$network->setUserSyncUrl(urlTemplate); 

```
Sample output: 

```
true
```

## Python Example {#section_dwg_gds_rz}


```
network.set_user_sync_url(urlTemplate) 

```
Sample output: 

```
True
```

## Ruby Example {#section_enh_gds_rz}


```
network.set_user_sync_url(urlTemplate) 

```
Sample output: 

```
True
```
