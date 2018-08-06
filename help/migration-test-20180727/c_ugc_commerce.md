---
description: Deliver product-specific UGC at specific points of the customer journey to increase purchase intent and conversion using the UGC Commerce feature.
seo-description: Deliver product-specific UGC at specific points of the customer journey to increase purchase intent and conversion using the UGC Commerce feature.
seo-title: UGC Commerce
solution: Experience Manager
title: UGC Commerce
uuid: ff2e67d1-2e05-443e-93b2-5b3f0bb0665a
index: y
internal: n
snippet: y
translate: y
---

# UGC Commerce

On this page:

* [](#c_ugc_commerce/section_s2d_tln_n1b)
* [](#c_ugc_commerce/section_n1s_4hz_m1b)
* [Using ModQ with UGC Commerce](#c_ugc_commerce/section_os1_v4t_n1b)
* [Using Streams with UGC Commerce](#c_ugc_commerce/section_qtj_v4t_n1b)
Use the UGC Commerce feature to influence purchase intent and conversion on UGC and product detail pages. Speed time to market by seamlessly associating UGC with product inventory. Build brand loyalty by creating community using UGC to highlight authentic customer stories.
AEM Livefyre provides several ways to import product catalog information, including SKU, thumbnail images, price, and product name. Easily manage the association of products with UGC by using AEM Livefyre’s rights requests, auto-stream rule tagging, and moderation workflows.
In addition to influencing purchasing, the capabilities in AEM Livefyre’s UGC commerce offering can be leveraged to drive conversions in other ways including:

* B2B lead generation: place Call-to-action buttons under UGC to capture leads
* B2C App downloads: prompt users to download an App
* Article referrals: link users to articles related to pieces of UGC
Place product call-to-actions alongside UGC to drive conversion. You can:

* Add product-specific UGC at scale to thousands of product detail pages.
* Embed AEM Livefyre’s visualization apps that support UGC commerce capabilities such as Media Wall and Mosaic on product detail pages.
* Use configurable referral tracking codes with an analytics solution to measure the conversions from product CTAs placed on UGC and UGC placed on product detail pages.
AEM Commerce users can seamlessly integrate their existing product catalog into Livefyre to drive user engagement in Livefyre's visualization Apps. Livefyre users who do not use AEM Commerce can manually import their product catalogs into Livefyre. See [Upload Products to Livefyre Using File Upload](#c_ugc_commerce/section_n1s_4hz_m1b), for more. 
Apps that use this feature:

* [Feature Card](c_feature_card_app.md#c_feature_card_app). For information on how to use UGC Commerce in a Feature Card, see [Feature Card Customizations](c_feature_card_app.md#section_uds_gzm_5y).
* [Filmstrip](c_filmstrip_app.md#concept_jpc_n2j_jbb). For information on how to use UGC Commerce in a Filmstrip, see [](c_filmstrip_app.md#section_ldf_sqc_vbb).
* [Media Wall](c_media_wall_app.md#c_media_wall_app). For information on how to use UGC Commerce in a Media Wall, see [Media Wall Customizations](r_media_wall_customizations.md#r_media_wall_customizations).
* [Mosaic](c_mosaic_app.md#c_mosaic_app). For information on how to use UGC Commerce in a Mosaic, see [Mosaic Customizations](r_mosaic_customizations.md#r_mosaic_customizations).

## Overview: How to use the UGC Commerce Call-to-action Button {#section_s2d_tln_n1b}


1. Create an App with a Call-to-action Button. See [Add an Action Button to an App](#c_ugc_commerce/section_wxx_xfz_31b).
1. Add your product catalog to Livefyre. You can import content in one of two ways:
    * [Import Products into Livefyre Using AEM Commerce](t_associate_products_with_ugc_using_aem_commerce.md#t_associate_products_with_ugc_using_aem_commerce) if you use AEM Commerce.
    * [Upload Products to Livefyre](#c_ugc_commerce/section_n1s_4hz_m1b) if you do not use AEM Commerce.

1. Associate products with content. You can do this in one of four ways:
    * From the Library. See [Associate Products with Content Using the Library](t_associate_products_with_content_using_the_library.md#t_associate_products_with_content_using_the_library)
    * From ModQ. See [Moderate Content Using ModQ](t_approve_content_from_modq.md#t_approve_content_from_modq)
    * From App Content. See [Add a Call-to-action Button to an App](t_add_a_call_to_action_button_to_an_app.md#t_add_a_call_to_action_button_to_an_app)
    * From a Stream. See [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).


## Upload Products to Livefyre Using File Upload {#section_n1s_4hz_m1b}

Upload products to use with your Call-to-Action Button to add products to associate with content or to edit and delete existing files.

>[!NOTE]
>
>Uploading a file into a folder with existing files will delete all the files in that folder and overwrite them with the new file.


1. Navigate to ** `Network Settings > Products.` **
1. Create a ** `Product Folder` ** or use an existing ** `Product Folder` **.
1. Click on the ** `Product Folder` ** to select it.
1. Click the ** `Upload Products` ** button.
1. Upload a product file in one of the following formats:
    * Google Products file format
    * Livefyre format (see below)
   Upload a JSON file in the standard format. You can download a template to see an example of the standard format. The following is an example of one product line in a template. It follows the sequence `{"key": "value", "key": "value"}, {"key": "value", "key": "value"}`: 

   ```
   {"id": "1", "title": "Flex RN 2017", "isFolder": false, "description": "Flex RN 2017", "price": "$85", "sku": "sku11111", "summary": "This brand is a member of the Sustainable Apparel Coalition", "features": "Cushioning: Lightweight, flexible response", "url": "www.shopping.com/shoes-flex-rn-2017/product/9", "attributes": [{"type": "color", "value": "blue"}
   ```
   The table explains the key and value pairs you need to upload products:

   #### Key/Value Pairs for Product Catalog Upload Standard Format
<table frame="all" rowsep="1" colsep="1" id="table_x41_fkv_n1b">
 <thead>
  <tr>
   <th class="entry">Key</th>
   <th class="entry">Type</th>
   <th class="entry">Description</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><span class="codeph">id</span></td>
   <td>String</td>
   <td>Unique ID of the product.</td>
  </tr>
  <tr>
   <td><span class="codeph">oembed</span></td>
   <td>Object</td>
   <td>Image attachment 0embed $ref: '../partials/schemas.yaml#/oEmbed'</td>
  </tr>
  <tr>
   <td><span class="codeph">title</span></td>
   <td>String</td>
   <td>Product title.</td>
  </tr>
  <tr>
   <td><span class="codeph">isFolder</span></td>
   <td>Boolean</td>
   <td>If true, the product is treated like a folder (for example, mens, womens, etc.).</td>
  </tr>
  <tr>
   <td><span class="codeph">parentId</span></td>
   <td>String</td>
   <td>Defines what folder the product is under.</td>
  </tr>
  <tr>
   <td><span class="codeph">description</span></td>
   <td>String</td>
   <td>Description of the product.</td>
  </tr>
  <tr>
   <td><span class="codeph">price</span></td>
   <td>String</td>
   <td>Value of the product in dollars. For example, '23.36.'</td>
  </tr>
  <tr>
   <td><span class="codeph">sku</span></td>
   <td>String</td>
   <td>Stock keeping unit (SKU) of the product.</td>
  </tr>
  <tr>
   <td><span class="codeph">url</span></td>
   <td>String</td>
   <td>Link to the product page.</td>
  </tr>
  <tr>
   <td><span class="codeph">enabled</span></td>
   <td>Boolean</td>
   <td>A value of True means the product is active.</td>
  </tr>
  <tr>
   <td><span class="codeph">attributes</span></td>
   <td>Array</td>
   <td><p>Types and values that define the product (for example, color, size, etc.). This is an array of objects.</p><p>Properties:</p>
    <ul id="ul_rkb_z3w_41b">
     <li><span class="codeph">type</span>
      <ul id="ul_j5z_zkw_41b"> 
       <li>Type: String</li> 
       <li>Description: Color, size</li> 
      </ul></li>
     <li><span class="codeph">value</span>
      <ul id="ul_pyh_blw_41b"> 
       <li>Type: String</li> 
       <li>Description: Green, XS</li> 
      </ul></li>
    </ul></td>
  </tr>
  <tr>
   <td><span class="codeph">tags</span></td>
   <td>Array</td>
   <td><p>Tags defining categories of content (for example, cars, shoes, etc.). This is an array of strings.</p></td>
  </tr>
 </tbody>
</table>




## ModQ {#section_os1_v4t_n1b}

You can associate content with products from your product catalog in ModQ in line with your existing moderation workflows. For information on how to use UGC Commerce with ModQ, see [Moderate Content Using ModQ](t_approve_content_from_modq.md#t_approve_content_from_modq).

## Streams {#section_qtj_v4t_n1b}

You can automatically associate products to content using stream rules, then publish the content automatically to an App, save it in the Library, or Moderate it using ModQ. For more information on how to use UGC Commerce with Stream Rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).
