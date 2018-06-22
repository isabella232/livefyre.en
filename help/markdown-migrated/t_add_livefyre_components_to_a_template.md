---
description: 
seo-description: 
seo-title: Add Livefyre Components to a Template
title: Add Livefyre Components to a Template
---

# Add Livefyre Components to a Template

>1. Access `uicontrol CRXDE Lite`.
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
