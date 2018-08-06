---
description: Allow customers to rate and review your product offerings.
seo-description: Allow customers to rate and review your product offerings.
seo-title: Reviews
solution: Experience Manager
title: Reviews
uuid: f432580a-a828-484d-b788-95147a700dd7
index: y
internal: n
snippet: y
translate: y
---

# Reviews

Reviews allows members of your community to contribute star ratings and qualitative reviews for any product or service.

## Integration {#section_kk5_15b_c1b}

To integrate a Reviews App, follow the procedure for Integrating a Conversation App. See [](c_implement_a_conversation_app.md#concept_zvy_c3c_tbb). The following is an example of an embedded Reviews App. 
**Example:** 

```
var networkConfig = { 
   network: "client-solutions-uat.fyre.co" 
}; 
  
var convConfig = { 
   siteId: '304059', 
   articleId: 'sh_col_22_1373478370_reviews', 
   el: 'livefyre-comments', 
   app: 'reviews', 
   ratingSummaryEnabled: true, 
   maxRating: 5, 
   collectionMeta: 'eyJhbGciOiAiSFMyNTYiLCAidHlwIjogIkpXVCJ9.eyJ1cmwiOiAiaHR0cDovL3d3dy5kaXJlY3R2LmNvbS9wZXJzb24vQW5uYS1QYXF1aW4tYjJGU0wwZHJLM051YldjOS1yZXZpZXdzIiwgInNpdGVJZCI6ICIzMDQwNTkiLCAiYXJ0aWNsZUlkIjogInNoX2NvbF8yMl8xMzczNDc4MzcwX3Jldmlld3MiLCAidHlwZSI6ICJyZXZpZXdzIiwgInRpdGxlIjogIlRCX1BhcXVpbl9yYXRpbmdzX3Jldmlld3MifQ.hes3KMwygCG-fFDQlkaB-XlxGjW6-iZ68xA4RRGqUl0' 
}; 
  
Livefyre.require(['fyre.conv#3'], function (Review) { 
   new Review(networkConfig, [convConfig], function (reviewWidget) {}); 
   auth.delegate({ 
      login: function (callback) { 
         callback(null,{livefyre:'<userauthtoken>'}); 
      }, 
   }); 
});
```
As noted in the Building ` CollectionMeta` section, ` CollectionMeta` is an encoded JSON object. In the above example, the JSON object takes the following format before it’s JWT encoded: 

```
{ 
"url": "http://www.directv.com/person/Anna-Paquin-b2FSL0drK3NubWc9-reviews",  
"siteId": "304059",  
"articleId": "sh_col_22_1373478370_reviews",  
"type": "reviews",  
"title": "TB_Paquin_ratings_reviews" 
}
```

## convConfig Object {#section_pzv_ytb_c1b}

If you’ve already completed the Getting Started section you should be familiar with convConfig object. To enable Reviews, update the convConfig with the following fields:

## Review Collection Metadata {#section_k1s_sqb_c1b}


>[!NOTE]
>
>To use ` ratingSubpartsIds`, the ` ratingSubparts` param must also be defined, and the length of the two arrays must match. 


```
networkConfig["strings"] = { 
   ratingSubpartPlaceholders: ['Pros...', 'Cons...'], 
   ratingSubpartTitles: ['Pros:', 'Cons:'], 
   ratingSubpartIds: ['pros', 'cons'], 
   reviewStreamTitle: 'Description:' 
} 
fyre.conv.load(networkConfig, [{ 
   app: 'reviews', 
   ratingSubparts: 2, 
    ... // More conv config settings 
}]);
```

>[!NOTE]
>
>If you’re using ` ratingDimensions`, you MUST use the ` ratingSelectionDelegate`, ` ratingDisplayDelegate`, and ` ratingSummaryDelegate` (if you want to show the rating summary). 


## Reviews Customization {#section_khz_xmb_c1b}

**Configure Star Images** 
To change the image for full stars, the class is “ ` goog-ratings-star`“. Change the background image to whatever image you’d like. By default, stars are 28 by 28 pixels. 
**Configure Star Images with Half Stars** 
With half stars, there are two classes, one for each side of the star. The left side of the half star is “ ` fyre-rating-half-odd`” and the right side is “ ` fyre-rating-half-even`“. By default, half stars are 28 by 14 pixels. 
**Configure the Tooltip Values for Stars** 
To configure the tooltip values for the stars, follow the custom text described in String Customizations. Once you have that set up, use the key “ ` ratingValues`” and the value an array that contains the tooltip strings. If you have half stars disabled, the number of elements in the array should be the same as ` maxRating` (above). If you have half stars enabled, the number of elements should be 2x ` maxRating`. The first element in the array corresponds to the left-most star (or half star) element and continues left to right. 
**Toggle the “Show My Review” Option** 
To toggle the “Show My Review” option on or off, target the ` hideShowReviewButton` parameter in the App configuration. 
**Show the Text Editor by Default** 
The reviews editor appears only after the user presses the “write review” button. To show this form by default, target the ` alwaysShowEditor` parameter in the App configuration. 
