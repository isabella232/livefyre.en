---
description: This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.
seo-description: This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.
seo-title: User Auth Token
solution: Experience Manager
title: User Auth Token
uuid: 4f2afd01-9a36-4513-9dfb-7fb78514f4c7
index: y
internal: n
snippet: y
translate: y
---

# User Auth Token

This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.

To create the token, use your preferred language library to pass in the following parameters:

|  Parameter  | Type  | Description  |
|---|---|---|
|  networkName  | String (required)  | The name of the Livefyre network (provided by Livefyre).  |
|  networkKey  | String (required)  | The secret key for this specific network (provided by Livefyre).  |
|  userId  | String (required)  | The ID of the user logging in as stored in your user management system (only alphanumeric, dash, underscore, and dot characters are allowed: [a-zA-Z0-9_-.]). **Note:** The userId must be unique.  |
|  expires  | Integer (required)  | When the token should expire from now (in seconds). **Note:** This value can also be passed as a float. The JSON web token produced will store this value in UNIX epoch time.  |
|  displayName  | String (required)  | Text to identify this user in the UI and in comments. (Maximum number of characters: 50.)  |


## Java {#section_b42_mjz_1cb}


```
network.buildUserAuthToken(userId, displayName, expires); 
 
```

## NodeJS {#section_c42_mjz_1cb}


```
network.buildUserAuthToken(userId, displayName, expires); 

```

## PHP {#section_d42_mjz_1cb}


```
$network->buildUserAuthToken(userId, displayName, expires); 

```

## Python {#section_e42_mjz_1cb}


```
network.build_user_auth_token(userId, displayName, expires) 

```

## Ruby {#section_f42_mjz_1cb}


```
network.build_user_auth_token(userId, displayName, expires) 

```

>[!NOTE]
>
>Network keys are not shared for Livefyre demosite accounts. You’ll receive a network key once Livefyre has provisioned an environment for you. This key should be kept private.

