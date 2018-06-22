---
description: A guide for building collectionMeta and auth tokens.
seo-description: A guide for building collectionMeta and auth tokens.
seo-title: Build Server Side Tokens
title: Build Server Side Tokens
---

# Build Server Side Tokens

Building the tokens that Livefyre uses to validate requests ensures that only you can make updates to your Livefyre network.

**CollectionMeta Token**

Learn how to build a token to create new and display existing conversations.

**Auth Token**

Learn how to build a token for authenticating users, a necessary step in the integration process if you’re not using Janrain Capture for user management.

## User Auth Token {#section_l5l_hwt_bbb}

This section describes how to generate the UserAuth JSON Object that creates the User Authentication token required to log users into your Apps.

To create the token, use your preferred language library to pass in the following parameters:

<table frame="all" rowsep="1" colsep="1" id="table_adq_qy5_nz"> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry">Parameter</th> 
    <th class="entry">Type</th> 
    <th class="entry">Description</th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>networkName</td> 
    <td>String (required)</td> 
    <td>The name of the Livefyre network (provided by Livefyre).</td> 
   </tr> 
   <tr> 
    <td>networkKey</td> 
    <td>String (required)</td> 
    <td>The secret key for this specific network (provided by Livefyre).</td> 
   </tr> 
   <tr> 
    <td>userId</td> 
    <td>String (required)</td> 
    <td>The ID of the user logging in as stored in your user management system (only alphanumeric, dash, underscore, and dot characters are allowed: [a-zA-Z0-9_-.]).<b>Note:</b> The userId must be unique.</td> 
   </tr> 
   <tr> 
    <td>expires</td> 
    <td>Integer (required) </td> 
    <td>When the token should expire from now (in seconds).<b>Note:</b> This value can also be passed as a float. The JSON web token produced will store this value in UNIX epoch time.</td> 
   </tr> 
   <tr> 
    <td>displayName</td> 
    <td>String (required)</td> 
    <td>Text to identify this user in the UI and in comments. (Maximum number of characters: 50.)</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

