---
description: When you implement Livefyre Apps, the style of implementation depends on your use case. This page explains the features for the three ways you can create an App.
seo-description: When you implement Livefyre Apps, the style of implementation depends on your use case. This page explains the features for the three ways you can create an App.
seo-title: CMS App Integrations
solution: Experience Manager
title: CMS App Integrations
uuid: ea3eaa5a-5301-4631-bb9e-504245972fb9
index: y
internal: n
snippet: y
---

# CMS App Integrations{#cms-app-integrations}

When you implement Livefyre Apps, the style of implementation depends on your use case. This page explains the features for the three ways you can create an App.

Livefyre integration is agnostic to any CMS and User Profile and Auth platform. Implement Livefyre in one or more ways, depending on your use-case and requirements.

You can use traditional integration to create customized AEM components.

#### CMS App Integration Type Overview
<table id="table_n4l_r4r_tz">  
 <thead> 
  <tr> 
   <th class="entry"> Type</th> 
   <th class="entry"> Development Requirement</th> 
   <th class="entry"> Features</th> 
   <th class="entry"> Pros </th> 
   <th class="entry"> Limitations</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> App Designer</td> 
   <td> Very Low</td> 
   <td> 
    <ul id="ul_o4l_r4r_tz"> 
     <li>Create JS embeds in Studio to add to pages without a developer</li> 
     <li>Limited Styling and Configurations available</li> 
     <li>Use case: Single Use Pages (event coverage, campaigns, hubs)</li> 
    </ul> </td> 
   <td> 
    <ul id="ul_mxj_qhw_sbb"> 
     <li>Able to get an App up and running in a short amount of time.</li> 
     <li>Configurations can be done by a non-technical member.</li> 
     <li>Easy on the fly changes to configurations</li> 
    </ul> </td> 
   <td> 
    <ul id="ul_j3h_bvk_rbb"> 
     <li>Must create an App using Livefyre Studio first</li> 
     <li>Not automated</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> Livefyre.js</td> 
   <td> Medium</td> 
   <td> 
    <ul id="ul_p4l_r4r_tz"> 
     <li>Integrate Apps into the JavaScript of your pages</li> 
     <li>Use case: Reusable templates (editorial content, product reviews)</li> 
    </ul> </td> 
   <td> 
    <ul id="ul_wk1_15k_rbb"> 
     <li>Use the full suite of App customizations and configurations</li> 
     <li>Automates the process to dynamically instantiate Apps from within your CMS onto your pages</li> 
    </ul> </td> 
   <td> 
    <ul id="ul_urm_ztk_rbb"> 
     <li>Need a developer up front. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> SDK APIs</td> 
   <td> Advanced</td> 
   <td> 
    <ul id="ul_q4l_r4r_tz"> 
     <li>Retrieve your content from Livefyre to use for custom applications</li> 
     <li>Customize front-end beyond out supported offering</li> 
     <li>Use case: Data/Analytics integrations and custom front-end apps</li> 
    </ul> </td> 
   <td> Full power over the look and feel of App</td> 
   <td> 
    <ul id="ul_dng_vhw_sbb"> 
     <li>Requires development up front.</li> 
     <li>Higher level of dev effort to implement.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

