---
description: This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.
seo-description: This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.
seo-title: Step 2: User Auth Token
title: Step 2: User Auth Token
---

# Step 2: User Auth Token

This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.

To create the token, use your preferred language library to pass in the following parameters:

<table frame="all" rowsep="1" colsep="1" id="table_adq_qy5_nz"> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry"> Parameter </th> 
    <th class="entry"> Type </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> networkName </td> 
    <td> String (required) </td> 
    <td> The name of the Livefyre network (provided by Livefyre). </td> 
   </tr> 
   <tr> 
    <td> networkKey </td> 
    <td> String (required) </td> 
    <td> The secret key for this specific network (provided by Livefyre). </td> 
   </tr> 
   <tr> 
    <td> userId </td> 
    <td> String (required) </td> 
    <td> The ID of the user logging in as stored in your user management system (only alphanumeric, dash, underscore, and dot characters are allowed: [a-zA-Z0-9_-.]). <b>Note:</b> The userId must be unique. </td> 
   </tr> 
   <tr> 
    <td> expires </td> 
    <td> Integer (required) </td> 
    <td> When the token should expire from now (in seconds). <b>Note:</b> This value can also be passed as a float. The JSON web token produced will store this value in UNIX epoch time. </td> 
   </tr> 
   <tr> 
    <td> displayName </td> 
    <td> String (required) </td> 
    <td> Text to identify this user in the UI and in comments. (Maximum number of characters: 50.) </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

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
$network-&gt;buildUserAuthToken(userId, displayName, expires); 

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
