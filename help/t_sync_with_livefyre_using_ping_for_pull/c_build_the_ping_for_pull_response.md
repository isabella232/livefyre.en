---
description: Build the Ping for Pull response to transmit updated user information to Livefyre.
seo-description: Build the Ping for Pull response to transmit updated user information to Livefyre.
seo-title: Build the Ping for Pull Response
solution: Experience Manager
title: Build the Ping for Pull Response
uuid: 23610b3e-aa10-4e33-b25a-7ea321947688
index: y
internal: n
snippet: y
translate: y
---

# Build the Ping for Pull Response

Build the Ping for Pull response to transmit updated user information to Livefyre.

<table frame="all" rowsep="1" colsep="1" id="table_lqg_n4r_tdb"> 
 <thead> 
  <tr> 
   <th class="entry"> Type</th> 
   <th class="entry"> Property</th> 
   <th class="entry"> Description</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> String (required)</td> 
   <td> <span class="parmname"> id</span> </td> 
   <td> The user ID of the user in your profile system. This must be unique across all users in your Network, and must never change.</td> 
  </tr> 
  <tr> 
   <td> String (required) </td> 
   <td> <span class="parmname"> display_name</span> </td> 
   <td> The display name of the user. This will be rendered with Livefyre Content posted by the user.</td> 
  </tr> 
  <tr> 
   <td> Object (optional, but recommended) </td> 
   <td> <span class="parmname"> name</span> </td> 
   <td> Strings to define the user’s formatted, first, middle, and last names.</td> 
  </tr> 
  <tr> 
   <td> String (optional, but recommended) </td> 
   <td> <span class="parmname"> email</span> </td> 
   <td> User’s email address. Used to send email notifications.</td> 
  </tr> 
  <tr> 
   <td> String (optional, but recommended) </td> 
   <td> <span class="parmname"> image_url</span> </td> 
   <td> <p>URL to an avatar to display for the user. Livefyre scales uploaded images to 100×100, 75×75, or 50×50 pixels, as appropriate. For best results, users should upload a square image, at 100×100 pixels.To ensure the avatar image is updated in Livefyre, modify the image_url for each image update so Ping for Pull detects that the image was changed. For example, attach a timestamp to the filename or increment the image changes.</p> <p>Note:  All URLs must be fully qualified and accessible.</p> </td> 
  </tr> 
  <tr> 
   <td> String (optional, but recommended) </td> 
   <td> <span class="parmname"> profile_url</span> </td> 
   <td> URL to the user’s profile page on your site.</td> 
  </tr> 
  <tr> 
   <td> String (optional, but recommended) </td> 
   <td> <span class="parmname"> settings_url</span> </td> 
   <td> URL to a page where users may configure the user’s profile settings for your site.</td> 
  </tr> 
  <tr> 
   <td> Array (optional, but recommended) </td> 
   <td> <span class="parmname"> tags </span> </td> 
   <td> Used to assign users to user groups. Tags may include 1-63 alphanumeric and underscore characters.</td> 
  </tr> 
  <tr> 
   <td> Boolean (optional, but recommended) </td> 
   <td> <span class="parmname"> autofollow_conversations</span> </td> 
   <td> Defines whether a user wishes to automatically follow a Collection after posting to it. When following a Collection, users receive email notifications when other users participate. May be true or false. Defaults to true.</td> 
  </tr> 
  <tr> 
   <td> Object (optional, but recommended) </td> 
   <td> <span class="parmname"> email_notifications</span> </td> 
   <td> <p>Defines the frequency of available Livefyre email notifications. Different frequencies may be set for each notification type. By default, no notifications will be sent.</p> 
    <ul id="ul_tyj_3jc_mz"> 
     <li> <span class="codeph"> immediately</span> issues notifications immediately upon the listed event.</li> 
     <li> <span class="codeph"> often</span> issues notifications in batches.</li> 
     <li> <span class="codeph"> never</span> will not send email notification for the activity.</li> 
    </ul> 
    <ul id="ul_ovk_zdb_mz"> 
     <li> <b>comments:</b> Defines when notifications are sent when other users post content into Collections that this user is following.</li> 
     <li> <b>replies:</b> Defines when notifications are sent when another user replies to this user’s content.</li> 
     <li> <b>likes:</b> Defines when notifications are sent when another user likes this user’s content.</li> 
     <li> <b>moderator_comments:</b> Defines when notifications are sent to moderators when users post content to any Collection in the Network.</li> 
     <li> <b>moderator_flags:</b> Defines when notifications are sent to moderators when other users flag content in any Collection in the Network.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> String (optional) </td> 
   <td> <span class="parmname"> location</span> </td> 
   <td> A user-submitted location.</td> 
  </tr> 
  <tr> 
   <td> String (optional) </td> 
   <td> <span class="parmname"> bio</span> </td> 
   <td> A user-submitted autobiography.</td> 
  </tr> 
  <tr> 
   <td> Array (optional) </td> 
   <td> <span class="parmname"> websites</span> </td> 
   <td> An array of user-submitted sites. Max = 2.</td> 
  </tr> 
  <tr> 
   <td> Object (optional) </td> 
   <td> <span class="parmname"> display_rules</span> </td> 
   <td> <p>Defines which profile properties are publicly visible to other users. Each available parameter takes Boolean input true or false. Available parameters: </p> 
    <ul id="ul_tsh_32d_mz"> 
     <li> <span class="codeph"> bio</span> </li> 
     <li> <span class="codeph"> location</span> </li> 
     <li> <span class="codeph"> gender</span> </li> 
     <li> <span class="codeph"> nameimage</span> </li> 
     <li> <span class="codeph"> remote_profile_url</span> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> Boolean (optional)</td> 
   <td> <span class="parmname"> moderator</span> </td> 
   <td> Defines whether the user has moderator privileges across the network.</td> 
  </tr> 
  <tr> 
   <td> Boolean (optional) </td> 
   <td> <span class="parmname"> gravatar_disabled</span> </td> 
   <td>Defines whether to disable Livefyre’s use of a gravatar if no <span class="codeph"> image_url</span> is provided.</td> 
  </tr> 
 </tbody> 
</table>

## Example Response {#section_uxt_3dd_mz}

```
{
 "id": "1234567890",
 "display_name": "Bob Dole",
 "name": {
   "formatted": "Bob Joseph Dole",
   "first": "Bob",
   "middle": "Joseph",
   "last": "Dole"
 },
   "email": "bob@dole.com",
   "image_url": "https://dole.com/images/bob.jpg",
   "profile_url": "https://site.com/bobdole",
   "settings_url":"https://site.com/settings",
   "tags": ["bob", "dole"],
   "autofollow_conversations": "true",
   "email_notifications": {
      "comments": "never",
      "replies": "immediately",
      "likes": "often",
      "moderator_comments": "immediately",
      "moderator_flags": "immediately" 
 },
  "location": "Washington D.C., USA",
  "bio": "Bob Dole speaks in the third person",
  "websites": ["https://dole.com/blog/", "https://bobdolerocks.com"],
  "display_rules": {
      "bio": "false",
      "location": "false",
      "gender": "false",
      "name": "false",
      "image": "false",
      "remote_profile_url": "false"
  },
  "moderator": "true",
  "gravatar_disabled": "false"
}
```

