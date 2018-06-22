---
description: AEM Commerce users can seamlessly integrate their existing product catalog into Livefyre to drive user engagement in Livefyre's visualization Apps.
seo-description: AEM Commerce users can seamlessly integrate their existing product catalog into Livefyre to drive user engagement in Livefyre's visualization Apps.
seo-title: Use HootSuite with AEM Livefyre
solution: Experience Manager
title: Use HootSuite with AEM Livefyre
---

# Use HootSuite with AEM Livefyre


>## Use AEM with Livefyre {#t_use_aem_for_livefyre}
>The Livefyre Adobe Experience Manager Package seamlessly integrates Livefyre’s industry-leading Social Depth Applications with your existing AEM site and creation tools.
<draft-comment author="ind14750" otherprops="merge">
 t_use_aem_for_livefyre.dita
</draft-comment>

On this page:

* [](#t_set_up_aem_for_livefyre)
* [](#c_before_you_begin_aem_livefyre)
* [](#install_livefyre_for_6.1_or_6.2)
* [](#t_install_livefyre_to_use_aem_assets)
* [](#t_configure_aem_to_use_livefyre)
* [](#t_customize_single_sign_on_integration)
* [](#t_integrate_aem_sites_and_communities)
* [](#t_add_livefyre_components_to_individual_pages)
* [](#t_enable_the_livefyre_cloud_service_for_a_page)
* [](#t_add_livefyre_components_to_a_page)
* [](#t_add_livefyre_components_to_a_template)
* [](#t_edit_a_livefyre_component_from_an_aem_page)
* [](#t_publish_a_livefyre_component_to_a_page)
* [](#t_import_ugc_content_into_aem_assets)
* [](#t_select_ugc_to_import_into_assets)
* [](#t_request_rights_using_aem_assets)
* [](#t_publish_ugc_in_aem_sites_or_communities)
* [](#t_associate_products_with_ugc_using_aem_commerce)
* [](#concept_xjh_dxk_1cb)
With AEM, you can discover and publish valuable user-generated content from social networks to your site in minutes, using Livefyre Apps. Features in using Livefyre with AEM include

* Automatic integration of AEM Identity Management with Livefyre’s Single Sign On capabilities.
* A suite of AEM components help your team publish Livefyre social content to your AEM sites and communities.
* Access to Livefyre Studio, including tools to discover, curate, organize, and publish your social content assets in real-time.
* Supports Touch or Classic UI for some versions of Livefyre with AEM.
* Supports AEM templates and JSP components.
See a video of how AEM and Livefyre work together:


>## Set Up AEM for Livefyre {#t_set_up_aem_for_livefyre}
>Follow this series of steps to install and configure AEM for Livefyre.

<!-- t_set_up_aem_for_livefyre.dita -->
To install and use an AEM Sites and Assets package you need AEM 6.2 GA or 6.3 GA. To set up AEM for Livefyre:

>1. Remove any previous instances of Livefyre in your AEM system.
>   
>1. Back up your data and current AEM instance.
>   
>1. Make sure you have all the items in [Before you Begin](c_before_you_begin_aem_livefyre.md#c_before_you_begin_aem_livefyre).
>   
>1. Perform one of the following tasks:
>    * [Install Livefyre for 6.1 or 6.2](t_install_livefyre_for_6.1_or_6.2.md#install_livefyre_for_6.1_or_6.2)
>    * [Install Livefyre to use AEM Assets](t_install_livefyre_to_use_aem_assets.md#t_install_livefyre_to_use_aem_assets)
>   
>1. [Configure AEM to Use Livefyre.](t_configure_aem_to_use_livefyre.md#t_configure_aem_to_use_livefyre)
>   
>1. (Optional)[Customize Single Sign-on Integration.](t_customize_single_sign_on_integration.md#t_customize_single_sign_on_integration)
>   
>   

>## Before you Begin {#c_before_you_begin_aem_livefyre}
>Ensure you have the items in this list in order to install and use AEM Communities.

<!-- t_set_up_aem_for_livefyre.dita -->
To install and use an AEM Communities Package, you will need:

* Adobe Experience Manager 6.1, 6.2 GA or 6.3 GA
    * If your organization is interested in using Livefyre with other versions of Adobe Experience Manager, [contact Livefyre](https://go.livefyre.com/contact) to let us know.
  
* AEM Communities for your version of AEM
    * For deployment options, see [Deploying Communities](https://docs.adobe.com/docs/en/aem/6-1/deploy/communities.html) on docs.adobe.com.
  
* A Livefyre license, and an account to access Livefyre Studio
    * If you already have a Livefyre license, your Account Manager can invite you to Livefyre Studio.
    * To learn more about Livefyre, [contact Livefyre](https://go.livefyre.com/contact) and tell us about your Social Content publishing needs. We can help!
  

>## Install Livefyre for AEM 6.1 or AEM 6.2 {#install_livefyre_for_6.1_or_6.2}
>Follow these steps to Install Livefyre for AEM 6.1 or 6.2 without AEM Assets.

<!-- install_livefyre_for_6.1_or_6.2.dita -->
For more information on downloading and installing AEM packages, see Downloading and Installing Packages from Package Share on docs.adobe.com.

To install the Livefyre for AEM package for 6.1 or 6.2:

>1. Search AEM Package Share for “Communities.”
>   
>1. Click on one of the following Communities Packages that contain the Livefyre package and automatically install Livefyre in AEM:
>* If using AEM 6.2, install the latest [AEM 6.2 Communities feature pack](https://docs.adobe.com/docs/en/aem/6-2/deploy/communities.html#Latest%20Feature%20Pack)
>* If using AEM 6.1, install the latest [AEM 6.1 Communities feature pack](https://docs.adobe.com/docs/en/aem/6-1/deploy/communities.html#Latest%20Feature%20Pack)
>* **Note:** You do not need to have a communities license to use AEM with Livefyre. You must have a Livefyre license to use AEM with Livefyre.
>   
>   
>1. Download the feature pack into Package Manager. Livefyre automatically installs when you install Communities. To check that Livefyre is active, you can view the bundle in the system console. For more information on how to view the bundle in the system console, see Web Console on docs.adobe.com.
>   
>1. Replicate the package to your Publish instance by clicking `uicontrol More &gt; Replicate`.
>   
>   

>## Install Livefyre to use AEM Assets {#t_install_livefyre_to_use_aem_assets}
>Follow the steps to install and use Livefyre with AEM Assets.

<!-- t_install_livefyre_to_use_aem_assets.dita -->
To install AEM Assets for use with Livefyre:

>1. Contact your sales consultant or account manager for the bundle and the package for your version of AEM (6.2 GA or 6.3 GA only).
>   
>1. Install the Livefyre bundle for your version AEM.
>   
>1. Install the AEM Assets and Sites package for your version of AEM.
>   >[!NOTE]
>   >
>   >You need to have an AEM Assets license to use AEM Assets with Livefyre. You must have a Livefyre license to use AEM Assets with Livefyre.
>   
>   
>1. Download the package into Package Manager. Livefyre automatically installs when you install the bundle and package. To check that Livefyre is active, you can view the bundle in the system console. For more information on how to view the bundle in the system console, see Web Console on docs.adobe.com.
>   
>1. Replicate the package to your Publish instance by clicking `uicontrol More &gt; Replicate`.
>   
>   

>## Configure AEM to Use Livefyre {#t_configure_aem_to_use_livefyre}
>Configure AEM to use your organization’s Livefyre license credentials.

>1. <!-- t_configure_aem_to_use_livefyre.dita -->
Find your organization’s Livefyre credentials. Open Livefyre Studio, and go to `uicontrol Settings &gt; Integration Settings &gt; Credentials`, to access the following information:
>* `uicontrol Network Domain`
>* `uicontrol Network Key`
>* `uicontrol Site ID`
>* `uicontrol Site Key`
>   
>   
>1. Configure AEM to use this Livefyre Network and Site by creating one or more Livefyre Cloud Service Configurations.
>   >1. From the AEM Dashboard, go to `uicontrol Tools &gt; Deployment &gt; Cloud Services`.
>   >   
>   >1. Scroll to the `uicontrol Livefyre` section.
>   >   
>   >1. Click `uicontrol Configure now`or `uicontrol Show Configurations`(depending on your AEM platform).
>   >   
>   >1. Click the plus sign (`uicontrol +`) next to `uicontrol Available Configurations` to create a Livefyre Configuration.
>   >   
>   >1. Complete the information. For more on how to complete the information for Livefyre in AEM Cloud Services, see the Cloud Services Documentation for AEM on docs.adobe.com.
>   >   
>   >   
>   
>1. When the `uicontrol Livefyre Network Configuration` form displays, enter the Network Domain, Network Key, Site ID, and Site Key you obtained from Studio, and click `uicontrol OK`.
>   If your AEM Publish and AEM Author do not share the same cryptographic key you may need to repeat this process on the publisher instances. This is because the Network Key and Site Key are encrypted. For more information, see Replicate the Crypto Key on docs.adobe.com.
>   
>   

>## Customize Single Sign-on Integration {#t_customize_single_sign_on_integration}
>The Livefyre for AEM package includes an out-of-the-box integration between AEM Identity Management’s User Profiles and Livefyre’s SSO service.

<!-- t_customize_single_sign_on_integration.dita -->
When users log into your AEM site, they are also logged into Livefyre social components, and when a logged-out user attempts to use a Livefyre component feature that requires authentication (like uploading a photo), the Livefyre component can initiate user authentication.

The default authentication integration may not be perfect for every site. To best match the authentication flow in your site templates, you may want to override the default Livefyre Authentication Delegate to meet your needs.

>1. Using CRXDE Lite, copy `codeph /libs/social/integrations/livefyre/components/authorizablecomponent/authclientlib` to `codeph /apps/social/integrations/livefyre/components/authorizablecomponent/authclientlib`
>   
>   
>1. Edit and save`codeph  /apps/social/integrations/livefyre/components/authorizablecomponent/authclientlib/auth.js` to implement a Livefyre Auth Delegate that meets your needs.
>   For more information on customizing an Auth Delegate, see Identity Integration on answers.livefyre.com.
>   
>   For more on AEM Clientlibs, see Using Client-Side Libraries on docs.adobe.com.
>   
>   
>   
>   

>## Integrate AEM Sites and Communities {#t_integrate_aem_sites_and_communities}
>Follow these steps to use Livefyre components with AEM Sites and Communities.

<!-- t_integrate_aem_sites_and_communities.dita -->
>1. Add Livefyre Components to Individual Pages or Add a Livefyre App to a Template
>   
>1. Edit a Livefyre App from an AEM Page
>   
>1. Publish a Livefyre App to a Page
>   
>   

>## Add Livefyre Components to Individual Pages {#t_add_livefyre_components_to_individual_pages}

<!-- t_add_livefyre_components_to_individual_pages.dita -->
After you install and configure the Livefyre for AEM package, you can add Livefyre social components to any AEM page.

To add Livefyre components to your page, the page must inherit a Livefyre Cloud Service configuration from its parent page or have the configuration added directly to the page.


>## Enable the Livefyre Cloud Service for a Page {#t_enable_the_livefyre_cloud_service_for_a_page}

>1. <!-- t_enable_the_livefyre_cloud_service_for_a_page.dita -->
Create a new page or edit an existing page. For more information on how to create and edit a page, see Authoring Pages on docs.adobe.com
>   
>1. Choose **Open Properties **to open the **Page Properties** dialog.
>   
>1. Click **Cloud Services**.
>   
>1. If you do not see a Livefyre Cloud Service Configuration, click **Add Configuration**, then click **Livefyre**.
>   
>1. If you have more than one Livefyre Configuration, choose the one you’d like to use for this page and its children.
>   
>1. Click the **checkmark** in the top-right corner of the dialog to save.
>   
>1. Enter Design Mode for the page to allow placement of Livefyre Components on the page. For more on how to use Design Mode for a page in AEM, see Configuring Components in Design Mode on docs.adobe.com.
>   
>1. In the **Edit****dialog **window, scroll down in the **Allowed Components** section to find **Livefyre**. You can enable all components in the category, or any combination of individual components. for more information on how to enable or disable components in AEM, see Configuring Components in Design Mode on docs.adobe.com.
>   
>   

>## Add Livefyre Components to a Page {#t_add_livefyre_components_to_a_page}
>Add Livefyre components to a page in AEM.

>1. <!-- t_add_livefyre_components_to_a_page.dita -->
From the `uicontrol Components` side panel, select `uicontrol Livefyre` from the pulldown menu to limit the list to available Livefyre components.
>   
>1. Select a Livefyre component, and drag it into position on your page.
>   
>1. Once added, Livefyre Components automatically create a fresh Livefyre App to store and stream the social content rendered by the component. This App will be created in the Livefyre site and network used in the Livefyre Cloud Service Configuration for the AEM Page.
>   >[!NOTE]
>   >
>   >Because a new, empty Livefyre App is created for each added Livefyre component, the component may render with very little content before you add content using Livefyre Studio. For more information on how to add content to a Livefyre App from a page, see Edit a Livefyre Component from an AEM Page.
>   For more information on how to insert a component, see Editing Page Content on docs.adobe.com.
>   
>   
>   
>   

>## Add Livefyre Components to a Template {#t_add_livefyre_components_to_a_template}

>1. <!-- t_add_livefyre_components_to_a_page.dita -->
Access `uicontrol CRXDE Lite`.
>   
>1. Navigate to your template node.
>   
>1. Create a node in the location in which you want your Livefyre component.
>   For more information see[Page Templates - Editable](https://docs.adobe.com/docs/en/aem/6-3/develop/templates/page-templates-editable.html) in the AEM 6.3 documentation.
>   
>1. In the `uicontrol Create Node` window, enter the following information:
>* **Name:** sling:resourceType
>* **Type:** nt:unstructured
>   
>   
>1. In the Properties table, add one of the following values to the Value field, depending on which App you would like to add to the template:
>* To use the Card App: **social/integrations/livefyre/components/card**
>* To use the Carousel App: **social/integrations/livefyre/components/carousel**
>* To use the Chat App: **social/integrations/livefyre/components/chat**
>* To use the Comments App: **social/integrations/livefyre/components/comments**
>* To use the Feature Card App: **social/integrations/livefyre/components/card**
>* To use the Live Blog App: **social/integrations/livefyre/components/liveblog**
>* To use the Map App: **social/integrations/livefyre/components/map**
>* To use the Mosaic App: **social/integrations/livefyre/components/mosaic**
>* To use the Media Wall App: **social/integrations/livefyre/components/mediawall**
>   
>   
>   

>## Edit a Livefyre Component from an AEM Page {#t_edit_a_livefyre_component_from_an_aem_page}

>[!NOTE]
>
>You can only configure or edit a Livefyre component in Livefyre Studio.
<!-- t_edit_a_livefyre_component_from_an_aem_page.dita -->
1. Click the Livefyre Component to configure.
1. Click the **Configure** item (wrench) to open the Configuration Dialog.
1. Click **Livefyre Studio** in the toolbar to open the App in Studio.
1. Modify the App in Studio.

>## Publish a Livefyre Component to a Page {#t_publish_a_livefyre_component_to_a_page}
>Follow these steps to publish a Livefyre Component to a page in AEM.
<draft-comment author="ind14750" otherprops="merge">
 t_publish_a_livefyre_component_to_a_page.dita
</draft-comment>

>1. Configure AEM to use Livefyre.
>   
>1. Enable the Livefyre Cloud Service for a Page
>   
>1. Add a Livefyre Component to a page.
>   
>1. Edit the App in Livefyre Studio to stream social content into the App.
>   
>1. Publish the AEM page to make the App available to your AEM site or community. For more information on how to publish pages using AEM, see Publishing Pages on docs.adobe.com.
>   
>   

>## Import UGC Content into AEM Assets {#t_import_ugc_content_into_aem_assets}
>You can import Twitter and Instagram user-generated content (UGC) from Livefyre Studio to AEM Assets using the UGC Importer.

<!-- t_import_ugc_content_into_aem_assets.dita -->
Import UGC content to AEM Assets by:

* Accessing your Livefyre Library.
* Searching real-time on Twitter and Instagram using Livefyre Social Search.
>[!NOTE]
>
>To select real-time content from Instagram in AEM Assets, you must set up social accounts in Livefyre. See Social Accounts for more information on how to set up social accounts in Livefyre.
To import assets into AEM, perform the following steps:

>1. Select UGC from your Livefyre Library or real-time from Twitter or Instagram. See Select UGC to Import into AEM Assets for information on how to select UGC.
>   
>1. Manage the rights on the UGC. See Request Rights Using AEM Assets for information on how to manage rights. You must have rights to the UGC content you import into AEM Assets. Grant rights by:
>* Sending a request to the social content owner.
>* Manually overriding rights status.
>   >[!NOTE]
>   >
>   >To perform a rights request in AEM Assets, you must set up Rights Management in Livefyre. See[](t_set_up_rights_management.md#t_set_up_rights_management) for more information on how to set up Rights Management in Livefyre.
>   
>   
>1. Click `uicontrol Import` to complete the import process.
>   
>1. Publish UGC using Livefyre components or AEM default components.
>   
>   

>## Select UGC to Import into Assets {#t_select_ugc_to_import_into_assets}
>Select content from your Livefyre Library or run real-time searches across Twitter and Instagram.

<!-- t_select_ugc_to_import_into_assets.dita -->
Selecting UGC content is the first step in importing UGC content to AEM Assets.

>1. Log in to AEM Assets library.
>   
>1. Click `uicontrol Create`, then `uicontrol Import UGC`.
>   
>1. Find content:
>* From Livefyre by clicking on the `uicontrol UGC Library` tab. Use the filters and search to find content from the UGC Library.
>* From Twitter and Instagram by clicking on the `uicontrol Twitter` or `uicontrol Instagram` tab and use the search or filters to find content.
>   
>   
>1. Click on the assets you want to import to AEM Assets. The assets you select are automatically counted and saved under the `uicontrol Selected` tab.
>   
>1. Review and confirm the UGC content to import. click on the `uicontrol Selected` tab.
>   
>1. Click `uicontrol Next`.
>   
>   

>## Request Rights Using AEM Assets {#t_request_rights_using_aem_assets}
>Request rights for assets you want to import from the UGC Library, Twitter, or Instagram.

<!-- t_request_rights_using_aem_assets.dita -->
You must select UGC to import into AEM Assets before you can request rights for those assets. You can:

* Send a message to the owners of multiple assets at a time by using `uicontrol Bulk Message`
* Override the rights for multiple assets at once using `uicontrol Bulk Attribute Content Rights`
* Choose whether you want to message the content owner or manually attribute content rights for each asset you selected using `uicontrol Custom Actions`.
>[!NOTE]
>
>If any content item previously had rights requested or granted in the Livefyre platform, the status of the rights request will reflect appropriately for the content item.
>[!NOTE]
>
>Overriding a rights request is stating that you own the content. Do not override a rights request without verifying that you own the content.
>   1.
>   Choose one of the following options under `uicontrol Actions in Bulk`:
>   
>* `uicontrol Bulk Message` to send a message to the owners of several assets at once
>* `uicontrol Bulk Attribute Content Rights` to override the rights for multiple assets at once
>* `uicontrol Custom Actions` to choose whether to message the asset owner or override the rights request for each, individual piece of content. If you choose `uicontrol Custom Actions`, send a rights request message or modify the message for a rights request under individual assets.
>   
>   
>1. Click `uicontrol Import`.
>   You can see the status of a pending Rights Request for an asset in Livefyre Studio.
>   
>   >[!NOTE]
>   >
>   >If content is pending a rights request, the asset will not display in AEM Assets until rights are granted. The asset automatically appears in AEM Assets when a rights request is granted.
>   
>   
>   

>## Publish UGC in AEM Sites or Communities {#t_publish_ugc_in_aem_sites_or_communities}
>Display UGC on your AEM site.

<!-- t_publish_ugc_in_aem_sites_or_communities.dita -->
You can use UGC in AEM Sites or Communities in one of two ways:

* To use the content with the Social Media information it came from (for example, to make a piece of Twitter content come with the data from Twitter as well as the Twitter logo), the content must be inside a Livefyre component on an AEM Site.
    * Note: Any UGC content published to a Livefyre component happens in real time and does not go through the AEM publish workflow.
  
* To use the content as media only (for example, to use a photo by itself on your site with no information about where it came from, like Twitter or Instagram), use the asset in an image component on an AEM Site. Video or text-only content is not supported outside of the UGC context.

>## Import Product Catalogs into Livefyre with AEM Commerce {#t_associate_products_with_ugc_using_aem_commerce}
>AEM Commerce users can seamlessly integrate their existing product catalog into Livefyre to drive user engagement in Livefyre's visualization Apps.

<!-- t_associate_products_with_ugc_using_aem_commerce.dita -->
After you import the product catalog, the products show up in real time in your Livefyre instance. If you edit or delete items in your AEM Commerce Product Catalog, the changes automatically update in Livefrye.

>1. Ensure you have the latest AEM with Livefyre package installed on your AEM instance. For more on how to set up AEM with Livefyre, see [Use AEM with Livefyre](t_use_aem_for_livefyre.md#t_use_aem_for_livefyre).
>   
>1. Log in to AEM.
>   
>1. Navigate to `uicontrol AEM Commerce`.
>   
>1. Create a new collection or use an existing collection.
>   
>1. Click on `uicontrol Collection Properties`.
>   
>1. Click `uicontrol Sync to Livefyre`.
>   
>   

>## Use HootSuite with AEM Livefyre {#concept_xjh_dxk_1cb}

You can use an AEM Livefyre App with Hootsuite to stream assets from your AEM Livefyre libraries into Hootsuite. For more information about using the AEM Livefyre App with Hootsuite, see [](https://apps.hootsuite.com/0/adobe-livefyre)

