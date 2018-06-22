---
---

<table id="properties_rqx_qcc_mz" relcolwidth="1.0* 1.11* 1.41*" class="simpletable properties" cellpadding="4" cellspacing="0"> 
 <thead class="prophead sthead"> 
  <th class="proptypehd">Type</th> 
  <th class="propvaluehd">Property</th> 
  <th class="propdeschd">Description</th> 
 </thead> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (required)</td> 
  <td class="propvalue stentry"><span class="parmname">id</span></td> 
  <td class="propdesc stentry">The user ID of the user in your profile system. This must be unique across all users in your Network, and must never change.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (required)</td> 
  <td class="propvalue stentry"><span class="parmname">display_name</span></td> 
  <td class="propdesc stentry">The display name of the user. This will be rendered with Livefyre Content posted by the user.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Object (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">name</span></td> 
  <td class="propdesc stentry">Strings to define the user’s formatted, first, middle, and last names.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">email</span></td> 
  <td class="propdesc stentry">User’s email address. Used to send email notifications.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">image_url</span></td> 
  <td class="propdesc stentry"> <p>URL to an avatar to display for the user. Livefyre scales uploaded images to 100×100, 75×75, or 50×50 pixels, as appropriate. For best results, users should upload a square image, at 100×100 pixels.To ensure the avatar image is updated in Livefyre, modify the image_url for each image update so Ping for Pull detects that the image was changed. For example, attach a timestamp to the filename or increment the image changes.</p> <p>Note: All URLs must be fully qualified and accessible.</p> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">profile_url</span></td> 
  <td class="propdesc stentry">URL to the user’s profile page on your site.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">settings_url</span></td> 
  <td class="propdesc stentry">URL to a page where users may configure the user’s profile settings for your site.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Array (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">tags</span></td> 
  <td class="propdesc stentry">Used to assign users to user groups. Tags may include 1-63 alphanumeric and underscore characters.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Boolean (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">autofollow_conversations</span></td> 
  <td class="propdesc stentry">Defines whether a user wishes to automatically follow a Collection after posting to it. When following a Collection, users receive email notifications when other users participate. May be true or false. Defaults to true.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Object (optional, but recommended)</td> 
  <td class="propvalue stentry"><span class="parmname">email_notifications</span></td> 
  <td class="propdesc stentry"> <p>Defines the frequency of available Livefyre email notifications. Different frequencies may be set for each notification type. By default, no notifications will be sent.</p> 
   <ul id="ul_tyj_3jc_mz"> 
    <li><span class="codeph">immediately</span> issues notifications immediately upon the listed event.</li> 
    <li><span class="codeph">often</span> issues notifications in batches.</li> 
    <li><span class="codeph">never</span> will not send email notification for the activity.</li> 
   </ul> 
   <ul id="ul_ovk_zdb_mz"> 
    <li><b>comments:</b> Defines when notifications are sent when other users post content into Collections that this user is following.</li> 
    <li><b>replies:</b> Defines when notifications are sent when another user replies to this user’s content.</li> 
    <li><b>likes:</b> Defines when notifications are sent when another user likes this user’s content.</li> 
    <li><b>moderator_comments:</b> Defines when notifications are sent to moderators when users post content to any Collection in the Network.</li> 
    <li><b>moderator_flags:</b> Defines when notifications are sent to moderators when other users flag content in any Collection in the Network.</li> 
   </ul> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">location</span></td> 
  <td class="propdesc stentry">A user-submitted location.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">String (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">bio</span></td> 
  <td class="propdesc stentry">A user-submitted autobiography.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Array (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">websites</span></td> 
  <td class="propdesc stentry">An array of user-submitted sites. Max = 2.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Object (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">display_rules</span></td> 
  <td class="propdesc stentry"> <p>Defines which profile properties are publicly visible to other users. Each available parameter takes Boolean input true or false. Available parameters:</p> 
   <ul id="ul_tsh_32d_mz"> 
    <li><span class="codeph">bio</span></li> 
    <li><span class="codeph">location</span></li> 
    <li><span class="codeph">gender</span></li> 
    <li><span class="codeph">nameimage</span></li> 
    <li><span class="codeph">remote_profile_url</span></li> 
   </ul> </td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Boolean (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">moderator</span></td> 
  <td class="propdesc stentry">Defines whether the user has moderator privileges across the network.</td> 
 </tr> 
 <tr class="property strow"> 
  <td class="proptype stentry">Boolean (optional)</td> 
  <td class="propvalue stentry"><span class="parmname">gravatar_disabled</span></td> 
  <td class="propdesc stentry">Defines whether to disable Livefyre’s use of a gravatar if no <span class="codeph">image_url</span> is provided.</td> 
 </tr> 
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
 "image_url": "http://dole.com/images/bob.jpg",
 "profile_url": "http://site.com/bobdole",
 "settings_url":"http://site.com/settings",
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
 "websites": ["http://dole.com/blog/", "http://bobdolerocks.com"],
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
