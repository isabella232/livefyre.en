---
description: null
seo-description: null
seo-title: Livefyre Package Release Notes for AEM
title: Livefyre Package Release Notes for AEM
uuid: 2ce8f0af-ba77-4f9f-9a3d-b21f3225d1e5
index: y
internal: n
snippet: y
translate: y
---

# Livefyre Package Release Notes for AEM

## Livefyre Package Release Notes for AEM {#topic_35655E4E8FA04869AA6BC9C3AF108798}Short Description
## Full Release Schedule {#section_61D9377941B748C587B02AF9F840DC68}



| AEM Version |Feature Pack Version |Release Date |Notes |
|---|---|---|---|
| AEM 6.4 |TBD |5/10/2018 |  |
| AEM 6.3 |[2.0.4](c_livefyre-aem-rel-notes.md#section_F713C8C9D6984416892A9F890BD82698)  |2/22/2018 |[Release notes](c_livefyre-aem-rel-notes.md#section_F713C8C9D6984416892A9F890BD82698)  |
| [2.0.2](c_livefyre-aem-rel-notes.md#section_E1E54EDB509E4A01BB78CC3BA6EABAFE)  |1/18/18 |[Release notes](c_livefyre-aem-rel-notes.md#section_E1E54EDB509E4A01BB78CC3BA6EABAFE)  |
| 2.0.1 |11/20/2017 |Release notes unavailable |
| 2.0.0 |10/5/2017 |Release notes unavailable |
| 1.2.0 |6/14/2017 |Release notes unavailable |
| AEM 6.2 |[2.0.4](c_livefyre-aem-rel-notes.md#section_F713C8C9D6984416892A9F890BD82698)  |2/22/2018 |[Release notes](c_livefyre-aem-rel-notes.md#section_F713C8C9D6984416892A9F890BD82698)  |
| [2.0.2](c_livefyre-aem-rel-notes.md#section_E1E54EDB509E4A01BB78CC3BA6EABAFE)  |1/18/18 |[Release notes](c_livefyre-aem-rel-notes.md#section_E1E54EDB509E4A01BB78CC3BA6EABAFE)  |
| 2.0.1 |11/20/2017 |Release notes unavailable |
| 2.0.0 |10/5/2017 |Release notes unavailable |
| 1.2.0 |6/14/2017 |Release notes unavailable |
| AEM 6.1 |- |- |No longer supported |
| AEM 6.0 |- |- |No longer supported |

For AEM feature pack release notes, [click here](https://helpx.adobe.com/experience-manager/6-3/release-notes/feature-packs-release-notes.html). 
For more information on AEM packages, see [How to Work With Packages](https://helpx.adobe.com/experience-manager/6-3/sites/administering/using/package-manager.html). 

## Livefyre Feature Pack 2.0.6 {#section_E180F2159CDA4B92B71C88AA591A9320}


* **Release date:**5/10/2018
* **For AEM versions:**6.4


<table id="table_B4665E1ADB144B03BEE0B0E93BB56FAA"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry">Type</th> 
   <th colname="col2" class="entry">Description</th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>New feature or improvement</p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_32FD14770E0C49F48792E8FC1210DE4D"> 
      <li id="li_CB72DFE763A44A6C8EE2C48DD1A9CB01">Added the ability to search UGC before setting up rights request social accounts in Livefyre. You must setup social accounts to request rights, or override the rights request if you own the content.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bug fix</p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_B02EA9791619445E9ED36F9B1C060C4A"> 
      <li id="li_AE8190B6D29B42F981A27A1C04D10A75">Fixed an issue where deleting a social account in Livefyre Studio used for rights request caused an error when loading the UGC library in AEM.</li> 
      <li id="li_9301D235188044949C7A2923164C32E8">Fixed an issue where asset count in Livefyre studio did not match asset count in the AEM UGC library.</li> 
      <li id="li_81D8ADDBA74D48B681DA001D94735A7A">Fixed an issue in the UGC library where filtered results displayed after the filter options were reset.</li> 
      <li id="li_01755FBBF3DD4017A39FA62F617803D1">Fixed an issue with AEM Commerce where call-to-action buttons redirected users to the incorrect URL.</li> 
      <li id="li_21401004763A4C9DAE215E4F4111C2DA">Fixed an issue in AEM (6.2) Sites where dragging and dropping multiple components into the parsys placeholder caused it to disappear.</li> 
      <li id="li_0E5E64199F1745109EB4CE98B9F121E1">Fixed an issue where 'Bulk attribute content rights' functionality did not function when importing assets with 'Rights Requested' status.</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Known Issues** 
*


## Livefyre Feature Pack 2.0.4 {#section_F713C8C9D6984416892A9F890BD82698}


* **Release date:**2/22/2018
* **For AEM versions:**6.3 and 6.2 (separate installers)

<!-- JIRA issues for 2.0.4 release: https://wiki.corp.adobe.com/display/lfprodeng/AEM+2018.2.15+Release --> 

<table id="table_85604193C5CB42BC9184B97688FE17A1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry">Type</th> 
   <th colname="col2" class="entry">Description</th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>New feature or improvement</p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_D6C0B8FC40694977B5075D5518A16233"> 
      <li id="li_9145995CD34A4694ADB39FE8F063680D">Added the ability to view next and previous cards when viewing UGC cards.</li> 
      <li id="li_CA7DDD2D4BAA4B8199898DC766D0A21F">Added information into the UI on implementing common query operators for UGC search.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bug fix</p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_F6BF1CC1F177428FAFFCD3512C2BA711"> 
      <li id="li_40D96FA777DE473097FA3783D1D7FB2B">Fixed an issue where AEM Rights Requests were being made over HTTP instead of HTTPS.</li> 
      <li id="li_524CE1D3DB5C46BD96894642D5EEC044">Fixed an issue causing social search functionality in UGC library to malfunction.</li> 
      <li id="li_A7261949B01C45D39C601A7DBAB39A83">Fixed an issue causing a <span class="codeph">SocialException</span> error when creating a new user in User Management. 
       <!--FYR-6709--> </li> 
      <li id="li_CA539C83F4B044DEAC9D888E62BFE938">Fixed an issue when searching in the UGC library where keyboard actions were enabled while the progress spinner spins.</li> 
      <li id="li_BE26AA132AF14036AEBB98BA2280EECE">Fixed an issue in UGC library where incorrect assets load after an invalid folder name search.</li> 
      <li id="li_07C62A613E7448D5A545D11FA298B13D">Fixed an issue in UGC library causing the import button and validation message to malfunction when entering 300+ characters in the text box.</li> 
      <li id="li_4E16C6037535488FAEA50A75B2D3FD3C">Fixed an issue in UGC library causing selected assets to disappear on refresh.</li> 
      <li id="li_13ADFC51A40C43C88320DB5085E82E39">Fixed an issue in UGC library causing the show/hide filter button to malfunction after multiple clicks.</li> 
      <li id="li_2F8A0DE117C34998927A13551DF5E3D1">Fixed an issue where Rights Requests messages were not being sent out via Twitter when importing UGC.</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>


**Known Issues** 
* Audio for auto-play videos in the UGC library continues to play after closing the popup window.
* Refreshing the page in UGC library after applying filters and then switching between tabs clears the filters but does not reset asset cards.


## Livefyre Feature Pack 2.0.2 {#section_E1E54EDB509E4A01BB78CC3BA6EABAFE}


* **Release date:**1/18/2018
* **For AEM versions:**6.3 and 6.2 (separate installers)

<!-- JIRA issues for 2.0.2 release: https://wiki.corp.adobe.com/display/lfprodeng/AEM.2018.01.18+Release --> 

<table id="table_51478910685E47CFB46928B41AE77302"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry">Type</th> 
   <th colname="col2" class="entry">Description</th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>New feature or improvement</p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_3D63E1719A514663949DFFBC22C487B2"> 
      <li id="li_71F2777EB64B4714A388AA7A5A817512">Added a unique identifier for UGC asset cards.</li> 
      <li id="li_9081AC7DBE884C63AFAD03FBED51E331">The Livefyre app Filmstrip is now a draggable component.</li> 
      <li id="li_67C76D821C914DE491AEB1C21FE0B428">Updated the search icon in UGC library to be clickable, setting a focus to the search field.</li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bug fix</p> </td> 
   <td colname="col2"> <p><b>Issues relating to Assets:</b> </p> <p> 
     <ul id="ul_6833883247EB48EB99EC89B5989BBA22"> 
      <li id="li_7A27B7892B8F48C0BFAAABDECEAD811F">Fixed an issue where authors were unable to create folders or files in Digital Asset Management after installing a Livefyre package.</li> 
      <li id="li_DFA7D2C276A84643BAF24EE8F67AAE72">Fixed an issue where total asset count in UGC library did not update properly on refresh.</li> 
      <li id="li_C3142B4E4F744EDAB9FFF8F05D1FEDB0">Fixed an issue with UGC search where the progress spinner was failing to display.</li> 
      <li id="li_49AA05C9F7D94B0E842C6B8C16E7B4B9">Fixed an issue with bulk Rights Requests where the text area was failing to display.</li> 
      <li id="li_E786C9D5A4A843B488782E896517629E">Fixed an issue with UGC assets missing a user description on the import page.</li> 
      <li id="li_11DC721013A940398B06D419927BF8DC">Fixed an issue in UGC search where assets with undefined descriptions were being displayed.</li> 
      <li id="li_53A3950654154A6D9EB6967C2A4E03BE">Fixed an issue where 'i' information icons did not display any information when manually attributing content rights.</li> 
      <li id="li_D13C225E2CDD4411839A4D38ED448407">Fixed an issue in UGC library where filter menu titles wouldn't display properly after clicking on the filter button.</li> 
      <li id="li_5742BA065A6044E19D969D82827D153B">Fixed an issue in UGC library where filtering cards by rating did not produce correct results.</li> 
      <li id="li_544AD83DE5D042F3BD1FB0163C87DEE3">Fixed an issue in UGC library causing the progress spinner to display twice.</li> 
      <li id="li_A720B675B44945EFB38A1A0887FE92C9">Fixed an issue in UGC filters where the alt text on card icons did not match the actual filter they describe.</li> 
      <li id="li_678AF00C804E464AB6C498A790B75026">Fixed an issue with filter options in Twitter UGC search where "Tweets With Media" produced no media tweets.</li> 
      <li id="li_D4D2A030EC0B4DE782DEDBF808E4F72C">Fixed an issue where some Twitter assets in UGC search were being incorrectly displayed as text instead of image assets.</li> 
      <li id="li_E02021A494574241B7007AA4167C2078">Fixed an issue in the UGC library where refreshing the page reset any previously-selected filters and selections.</li> 
     </ul> </p> <p><b>Issues relating to Sites:</b> </p> <p> 
     <ul id="ul_3C0CC7D3E71D4008B1AFA14B01916B65"> 
      <li id="li_03209C041DA24028BFFE43CFB3037226">Fixed an issue where dragging a Livefyre component onto a site with no cloud configuration would fail without showing an error.</li> 
      <li id="li_9FD811297A314949A59A068321A07122">Fixed an issue causing an error when signing in to the Livefyre apps.</li> 
      <li id="li_83D99859F50C42C787F60B8B64D646BD">Fixed an issue causing the Livefyre upload button to malfunction.</li> 
      <li id="li_DA440D705207474ABC65C40619094E75">Fixed a sizing issue with the Livefyre Map component.</li> 
      <li id="li_26EE155BBDA04B33A42063DBC08FDAE0">Fixed an issue with the Livefyre Liveblog component where the UI did not properly render.</li> 
     </ul> </p> <p><b>Issues relating to Firefox browser:</b> </p> <p> 
     <ul id="ul_45FAFE71C2074AE891F470DD2A51484F"> 
      <li id="li_2BFA25F8C5D142A8BEA9615D24590432">Fixed an issue where Livefyre components added to a site with Firefox browser necessitated an external refresh to render.</li> 
      <li id="li_DFC9E56C75C64968BEFA91A8DDE5B71D">Fixed an issue where using Firefox to embed existing apps produced an error.</li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>


**Known Issues** 
* Keyboard actions while searching in the UGC library are incorrectly enabled while the progress spinner spins.
* Assets in UGC library load incorrectly after an invalid folder name search.
* Import button and validation message in UGC library malfunctions when entering 300+ characters in the text box.

