---
description: The NetworkConfig object is a JSON object that customizes the authentication system for network users.
seo-description: The NetworkConfig object is a JSON object that customizes the authentication system for network users.
seo-title: NetworkConfig Object
solution: Experience Manager
title: NetworkConfig Object
---

# NetworkConfig Object

The `codeph NetworkConfig` object is a JSON object containing the following parameters:

<table frame="all" rowsep="1" colsep="1" id="table_q4j_xx5_nz"> 
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
    <td><span class="varname">authDelegate</span></td> 
    <td>Object (required)</td> 
    <td>Used to customize the authentication system for custom network users.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">network</span></td> 
    <td>String (required)</td> 
    <td>A Livefyre-provided network name. For example: <i>yourname.fyre.co.</i></td> 
   </tr> 
   <tr> 
    <td><span class="varname">attachmentDelegate</span></td> 
    <td>Object (optional)</td> 
    <td>Used to specify the types of media attachments visible in the App stream. For more information, see Restricting Media.</td> 
   </tr> 
   <tr> 
    <td><span class="varname">strings</span></td> 
    <td>Object (optional)</td> 
    <td>Used to customize text strings of the HTML elements in any of the Livefyre Core Apps. For more information, see String Customizations.</td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

