---
description: null
seo-description: null
seo-title: Use Livefyre with AEM Sites
title: Use Livefyre with AEM Sites
uuid: 870ccc4f-6d0d-414a-91bb-5128d74de73f
index: y
internal: n
snippet: y
translate: y
---

# Use Livefyre with AEM Sites

## Use Livefyre with AEM Sites {#concept_B692627E41D942219A07A469EB0DD35F}Short DescriptionThe Livefyre with AEM Sites workflow includes:

1. [Add Livefyre Components to a Page](c_livefyre-aem-sites.md#task_0696D92E3C5A4B0A80A80863A7EA08B0)
1. [Edit a Livefyre Component from an AEM Page](c_livefyre-aem-sites.md#task_2E6BB9FCCA0C4103878F2DE1D855D884)


>[!NOTE]
>
>Screenshots were taken using the AEM 6.3 Touch UI.


>## Add Livefyre Components to a Page {#task_0696D92E3C5A4B0A80A80863A7EA08B0}Before adding Livefyre components to a page within Sites, you must enable Livefyre for the page by either inheriting a Livefyre cloud configuration from a parent page or by adding the configuration directly to the page. Refer to your implementation for how to include cloud services on your site.
Once Livefyre is enabled for the page, containers must be configured to allow Livefyre components. See [Configuring Components in Design Mode](https://helpx.adobe.com/experience-manager/6-3/sites/authoring/using/default-components-designmode.html) for instructions on how to enable different components. 

>[!NOTE]
>
>Apps requiring authentication to post will not function until authentication is configured in[Customize Single Sign-on Integration](c_livefyre-aem.md#task_E918244666C24EE0932137373B0731EA). 



>1. From the ** `Components` ** side panel in design mode, select ** `Livefyre` ** from the pulldown menu to limit the list to available Livefyre components.
>   ![](images/livefyre-add.png)>
>1. Select a Livefyre component, and drag it into position on your page.
>1. Select whether to create a new Livefyre app or to embed an existing one.

>       For more information on inserting components, see [Editing Page Content](https://helpx.adobe.com/experience-manager/6-3/sites/authoring/using/editing-content.html). 
>## Edit a Livefyre Component from an AEM Page {#task_2E6BB9FCCA0C4103878F2DE1D855D884}You can only configure and edit a Livefyre component in Livefyre Studio. From AEM:

>1. Click the Livefyre component to configure.
>1. Click the ** `Configure` ** icon (wrench) to open the configuration dialog.
>1. Click ** `To edit this component, go to Livefyre Studio` **.
>1. Edit the App in Livefyre Studio.
