---
description: Informs Livefyre to pull user information from a previously set user sync URL. Returns a Boolean.
seo-description: Informs Livefyre to pull user information from a previously set user sync URL. Returns a Boolean.
seo-title: syncUser Network Method
solution: Experience Manager
title: syncUser Network Method
uuid: 6d0f2547-6bfa-4f51-99bc-4230394b6d33
index: y
internal: n
snippet: y
translate: y
---

# syncUser Network Method


|  *` userId`* | String  | The user ID to sync with Livefyre. You must have a user sync URL set with Livefyre before calling this method.  |
|---|---|---|


## Java Example {#section_nyl_ycs_rz}


```
network.syncUser(userId); 

```
Sample output: 

```
true
```

## NodeJS Example {#section_xkd_gds_rz}


```
network.syncUser(userId); 

```
Sample output: 

```
true
```

## PHP Example {#section_ghf_gds_rz}


```
$network->syncUser(userId); 

```
Sample output: 

```
true
```

## Python Example {#section_dwg_gds_rz}


```
network.sync_user(userId) 

```
Sample output: 

```
True
```

## Ruby Example {#section_enh_gds_rz}


```
network.sync_user(userId) 

```
Sample output: 

```
True
```
