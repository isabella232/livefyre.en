---
description: Release Notes for the October 5, 2017 release.
seo-description: Release Notes for the October 5, 2017 release.
seo-title: October 5, 2017
title: October 5, 2017
---

# October 5, 2017

<table id="table_tth_dwn_lbb"> 
 <title>Production Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Issue Type</b> </th> 
    <th class="entry"> <b>Component</b> </th> 
    <th class="entry"> <b>Release Note</b> </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Bug</td> 
    <td>Livefyre Identity</td> 
    <td>Customers using Livefyre identity to login were experiencing issues seeing or updating their avatars when posting to commenting apps. This has been fixed now, as avatars are now visible and available for updating.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Rights Management</td> 
    <td>Fixed a bug with displaying long usernames in the Rights Modal tab.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Streams</td> 
    <td>Added the ability to hit the tab key in a Streams text field to complete a search term.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

<table id="table_gy3_vyn_lbb"> 
 <title>UAT Release</title> 
 <tgroup cols="3"> 
  <colspec colnum="1" colname="col1" /> 
  <colspec colnum="2" colname="col2" /> 
  <colspec colnum="3" colname="col3" /> 
  <thead> 
   <tr> 
    <th class="entry"> <b>Issue Type</b> </th> 
    <th class="entry"> <b>Component</b> </th> 
    <th class="entry"> <b>Release Note</b> </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td>Enhancement</td> 
    <td>Filmstrip</td> 
    <td>When a customer deploys a film strip app, newly streamed UGC will have a "new" label next to it to quickly identify them.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Filmstrip</td> 
    <td>Filmstrip is a brand new visualization App, primarily designed to showcase UGC in e-commerce scenarios, such as product pages or transactional websites. Film Strip horizontally aligns UGC to be displayed as a camera roll, one piece at the time. End users can navigate Filmstrip by clicking the side arrows to scroll through the content available.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Library</td> 
    <td>Files uploaded into the library by a customer will be automatically rights granted. This is a helpful feature when the users have turned on the "require rights granted" filter in their apps.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Livefyre Identity</td> 
    <td>Customers can now use their Github credentials to login into LIvefyre Identity and participate in our commenting apps.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Rights Management</td> 
    <td>Fixed a bug that allowed insertion of unicode characters in Rights Request messages to bypass validation.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>SAFE</td> 
    <td>Minor improvements added to SAFE Spam detection.</td> 
   </tr> 
   <tr> 
    <td>Bug</td> 
    <td>Service</td> 
    <td>Users without valid emails have emails constructed for them. Fixed an issue with production logs where the system did not send emails to these users.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>Studio</td> 
    <td>Updated the Livefyre Help link in the top navigation bar.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>UGC Commerce</td> 
    <td>As a customer I can now create a single Livefyre app (Mosaic, FilmStrip or Media Wall) and embed it in multiple product pages, that dynamically filters the appropriate UGC for each product page (example UGC with shoes for a Shoe product page).</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>UGC Commerce</td> 
    <td>Customers can now manually upload a google product catalogue into Livefyre studio using a JSON file export. This enables the customer to pair UGC with products from that catalogue and visualize them in our commerce enabled apps.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>UGC Commerce</td> 
    <td>Customers can select which product folders they want to use when filtering their E-commerce app by product ID. For example I want my new filmstrip to appear in my women's shoes and women bags product pages, therefore I will select only the "Women's shoes collection" and "Women's bags" product folders.</td> 
   </tr> 
   <tr> 
    <td>Enhancement</td> 
    <td>UGC Commerce</td> 
    <td>Livefyre customers can now filter the UGC published to their apps only if they have been rights granted. For example a customer can curate and publish a selection of items, but those items will only be rendered in the app once they have been rights granted by the author. This is particularly important for E-commerce use cases, where the UGC is used for commercial purposes.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

