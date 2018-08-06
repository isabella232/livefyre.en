---
description: Livefyre uses a PUSH interface to send an external system information about changes to user permissions.
seo-description: Livefyre uses a PUSH interface to send an external system information about changes to user permissions.
seo-title: Posting User Permissions to External Systems (Optional)
solution: Experience Manager
title: Posting User Permissions to External Systems (Optional)
uuid: 39fd69d0-25d6-4a4d-9679-5e35bcf0fb42
index: y
internal: n
snippet: y
translate: y
---

# Posting User Permissions to External Systems (Optional)


#### Types of Users in Livefyre Studio
<table frame="all" rowsep="1" colsep="1" id="table_trz_nxf_gz">  
 <thead> 
  <tr> 
   <th class="entry">User Type</th> 
   <th class="entry">Description</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td><b>owner</b></td> 
   <td> <p>This user is an owner, and can both moderate content, and assign new moderators.</p> </td> 
  </tr> 
  <tr> 
   <td><b>admin</b></td> 
   <td> <p>This user is a moderator, and can moderate content.</p> </td> 
  </tr> 
  <tr> 
   <td><b>member</b></td> 
   <td> <p>This user is whitelisted. Posted content does not pass through spam or profanity filters, and does not require approval in pre-moderated streams.</p> </td> 
  </tr> 
  <tr> 
   <td><b>none</b></td> 
   <td> <p>This user is a standard user, and has no special permissions.</p> </td> 
  </tr> 
  <tr> 
   <td><b>outcast</b></td> 
   <td> <p>This user has been banned from participating in any conversations.</p> </td> 
  </tr> 
 </tbody> 
</table>

To post user permissions to external systems, you must register a URL that receives permissions data as POST requests.
For example:

```
POST https://{networkName}.quill.fyre.co/?actor_token={token}&amp;push_affiliation_url={url}
```

<table frame="all" rowsep="1" colsep="1" id="table_cgn_xxf_gz"> 
 <thead> 
  <tr> 
   <th class="entry">Parameter</th> 
   <th class="entry">Description</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td><b>networkName</b></td> 
   <td> <p>Your Livefyre provided network name.</p> </td> 
  </tr> 
  <tr> 
   <td><b>token</b></td> 
   <td> <p>Valid system token.</p> </td> 
  </tr> 
  <tr> 
   <td><b>url</b></td> 
   <td> <p>URL to register.</p> </td> 
  </tr> 
 </tbody> 
</table>

The URL registered should accept POSTs with the following data as content-type: application/x-www-form-urlencoded.

<table frame="all" rowsep="1" colsep="1" id="table_obz_1yf_gz"> 
 <thead> 
  <tr> 
   <th class="entry">Parameter</th> 
   <th class="entry">Description</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td><b>jid</b></td> 
   <td> <p>JID of the user whose affiliation is changed. A JID is a string of the form user_id@network.</p> </td> 
  </tr> 
  <tr> 
   <td><b>affiliation</b></td> 
   <td> <p>Name of the permissions assigned, which must be one of the following: <span class="keyword">{admin | member | none | outcast | owner}</span></p> </td> 
  </tr> 
 </tbody> 
</table>

For additional information on updating user affiliation settings, see the [Add User Affiliation API Reference](http://api.livefyre.com/docs/apis/by-category/user-management#operation=urn:livefyre:apis:quill:operations:api:v3.0:affiliation:add:method=post).
