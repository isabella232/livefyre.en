---
description: Returns an encrypted user authenticated token for the network it is called from.
seo-description: Returns an encrypted user authenticated token for the network it is called from.
seo-title: buildUserAuthToken Network Method
solution: Experience Manager
title: buildUserAuthToken Network Method
uuid: 8828d356-c3c6-46a6-91bf-83bd59e35050

---

# buildUserAuthToken Network Method{#builduserauthtoken-network-method}

Returns an encrypted user authenticated token for the network it is called from.

|Variable|Type|Description|
|--- |--- |--- |
|userId|String|The user ID for the user to whom this token belongs.|
|displayName|String|The display name for the user.|
|expires|Double|When the token should expire in seconds.|

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
