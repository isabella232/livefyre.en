---
description: Change the size, width, and interaction options of the Carousel app.
seo-description: Change the size, width, and interaction options of the Carousel app.
seo-title: Customize a Carousel Using Studio
solution: Experience Manager
title: Customize a Carousel Using Studio
---

# Customize a Carousel Using Studio

All Apps use `uicontrol Style` and `uicontrol Config` options in the `uicontrol App Designer`. See Customizing Apps for details on the standard `uicontrol Style` and `uicontrol Config` options for all Apps in the `uicontrol App Designer`.

You can customize a Carousel using the following additional options in the App Designer:

  *
  `uicontrol Max Number of Items`
  
  Sets the number of items to be displayed in the Carousel. Default is 50.
  
  
  *
  `uicontrol Orientation`
  
  `uicontrol Responsive`. For computer screens only
  
    * If the content is larger than 600 pixels, displays horizontally
    * If the content is smaller than 600 pixels, displays vertically
    * **Vertical.** For computer screens or mobile devices. In mobile devices, the card shrinks to fit the size of the screen.
  
* `uicontrol Call-to-action button`
  You can use the Call-to-action button with a product catalog to direct users to a product or to your site for further action.
  
    * `uicontrol Call-to-action button`
      Switch the toggle to on to display the call-to-action button.
      
      
    * `uicontrol Require rights to display products`
      Switch the toggle to on to require that the content owner has granted rights for the content before a call-to-action button appears for the content.
      
      >[!NOTE]
      >
      >The content displays even if rights are not granted for the content, but the call-to-action button will not display with the content unless rights for the content are granted.
      
    * `uicontrol Show call-to-action in tile`. Choose whether to display the call-to-action button on a tile instead of displaying the call-to-action button only when the site visitor clicks on a card and opens the content in a larger window.
    * `uicontrol Call-to-action indication text`
      The text to display to prompt the user to click on the card to open the call-to-action modal.
      
      
    * `uicontrol Call-to-action header text`
      The words to display in the header above the Call-to-action button in the content modal. Default text is, "Shop these products:".
      
      
    * `uicontrol Call-to-action button text`
      The words to display in the Call-to-action button in the content modal. Default text is, "Buy Now:".
      
      
    * `uicontrol Product display options`
      Choose whether you want to display the `uicontrol Photo` and the `uicontrol Product name` with the Call-to-action button.
      
      >[!NOTE]
      >
      >Both the Photo and Product name buttons highlight blue when they are enabled.
      
    * `uicontrol Product URL referral tracking`
      Switch the toggle to on to track referrals from this App to the associated product page.
      
      
    * `uicontrol Referral tracking key-value pairs`
      Add parameters to further specify the referral tracking from your App content to the associated product page.
      
      
  
* `uicontrol Embed App in multiple pages`.
    * `uicontrol Filter UGC by Product ID`. Select this option to create one App for multiple product pages. Filter product-specific UGC to the App for each product page. You can select one or more folders to associate specific collections to the App.
    * `uicontrol Select Product folders`. Select the top-level product folders to use to filter UGC. Use CTRL/Command + click to select more than one folder. Livefyre uses the folder to determine which products in that folder to display in the App on various pages.
    * `uicontrol Show related content`. Toggle this to display content published to the App, but tagged with a different product ID. After the product-specific content for the App displays, Livefyre displays content for other products and content not associated with a product. Livefyre prioritizes the content with the same product ID first, then content published to the App with other product IDs, then content published to the App with no product IDs.
  
