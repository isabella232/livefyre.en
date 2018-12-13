---
description: Insert Ads in your Comments stream.
seo-description: Insert Ads in your Comments stream.
seo-title: Ads in Comments
solution: Experience Manager
title: Ads in Comments
uuid: f8d6372f-4468-4884-a384-116180b4c748

---

# Ads in Comments{#ads-in-comments}

Insert Ads in your Comments stream.

## Ads in Comments {#topic_CDD2ACF16AED4DE782725EE90089C04E}

Insert Ads in your Comments stream. 

The Livefyre Ads in Comments feature allows you to inject ads into your comment stream, define the frequency with which the ads will appear in the stream, and to create both synchronous and asynchronous ad injection delegates.

Livefyre provides the container through which you may inject an ad, using your Ad Management Solution provider.

To inject an ad, pass Livefyre two values:

* The frequency at which the advertisement should be injected into the Comment Stream 
* A function that serves the appropriate advertisement.

>[!NOTE]
>
>Ads will be rendered only when the ad placement is in the viewport. Ads will be shown only after parent comments (not within threads), and users will not be able to comment on these advertisements. This API does not allow you to specify the size of the element into which your ads will be placed.

## Integration {#concept_C99029E618EC49779E3117D2C303E4F1}

To use this feature, create a div element on the page into which the ads will be placed, then pass in the HTML from your ad provider.

Livefyre provides two ad placement types: synchronous, and asynchronous. Both types load your ads only when the user scrolls the page such that the ad's position is in view. Both also require that you return a DOM element (IFrame or div).

To obtain the ad, the synchronous method calls to a local repository, whereas asynchronous calls to an external service.

### Synchronous

To create a synchronous placement, include the ad in the delegate, and return the ad element itself. The synchronous method calls to a local repository, allowing you to handle your own ad generation.

### Asynchronous

The asynchronous method requires that the element be inserted in the DOM before you call to the ad provider. Your provider then determines which ad to send, and returns it.

To implement asynchronous ads, create a delegate which returns a element in which the ad will be placed, and a callback that will perform the placement of the ad. The element returned in the delegate must have a unique id for the ad to target. The callback will insert the ad into the element provided by the unique id.

>[!NOTE]
>
>Depending on your ad provider, the callback will behave differently.

When the page loads, Ads in Comments will hit the delegate, inject the element, then call the callback which updates the (previously defined) element with the ad. 

## Parameters {#concept_D7E27B0C21EF405C8EB826083DBB53EC}

The following parameters are available for use with this call.

For the ad object:

* **delay:** **(optional) integer** - Sets the number of comments after which the first ad will be displayed. Default is 10. 
* **frequency:(optional) integer** - Sets the number of comments after which each subsequent ad will be displayed. For example: Enter 2 to display an ad as every third comment. Default is 10. 
* **delegate:** ***required* function** - The function called to inject ads into the Comment stream.

The delegate object supports both synchronous and asynchronous ad invocations. The parameter being given to the delegate function, data, will contain:

* **title:** **string** - The title of the Collection. 
* **tags:** **array** - A list of tags associated with the Collection. 
* **id:** **string** - The article identifier of the Collection. 
* **url:** **string** - The URL of the Collection. 
* **networkId:** **string** - The network ID for the Collection. 
* **siteId:** **int** - The site ID for the Collection.

These items are passed in through the convConfig object in our example and are explained in more detail in our [Getting Started](../../c-app-integrations/c-comments-integration/c-comments-integration.md#section_656AAC97903F485084650269A6C7EBCE) section.

### Synchronous

The delegate returns an object containing:

* **element:** ***required* DOM element** - The element containing the ad to be inserted into the App.

**Asynchronous**: The delegate returns an object containing: The delegate returns an object containing two properties: element and callback:

* **element:** ***required* DOM element** - The element containing the ad to be inserted into the App. 
* **callback:** ***required* function** - The callback that will handle the insertion of the ad into the DOM element above.

For the `Conv` object, you can pass in a string to denote the title for the ad section:

* **strings:** **(optional)** - Used to customize the header text for your ads. 'Sponsored' by default.

## Synchronous Example {#concept_E733E4431D9948638B8102ADE398735F}

```
<script src="//cdn.livefyre.com/Livefyre.js"></script> 
<div id="livefyre-app-17"></div> 
<script> 
  
(function() { 
  var nextSlotId = 1; 
  function generateNextSlotName() { 
    var id = nextSlotId++; 
    return 'adslot' + id; 
  } 
  Livefyre.require(['fyre.conv#qa'], function(Conv) { 
    new Conv({ 
      network: 'qa-0.fyre.co', 
        env: 'qa', 
        strings: { 
          'sponsored': 'Sponsored by: Livefyre' 
        } 
      }, [{ 
        app: 'main', 
        siteId: '291206', 
        articleId: '17', 
        el: 'livefyre-app-17', 
        ad: { 
          delay: 5, 
          frequency: 10, 
          delegate: function(data) { 
            var elem = document.createElement('div'); 
            elem.id = generateNextSlotName(); 
            return { 
              element: elem 
            }; 
          } 
        } 
      }], function (widget) { 
        // Initialize or Auth 
      }); 
    }); 
}()); 
</script>
```

## Asynchronous Example {#concept_16B798C7EB20423DAA53ACCC71540051}

```
<script src="//cdn.livefyre.com/Livefyre.js"></script> 
<div id="livefyre-app-17"></div> 
<script> 
  
(function() { 
  var nextSlotId = 1; 
  function generateNextSlotName() { 
    var id = nextSlotId++; 
    return 'adslot' + id; 
  } 
  function insertSlot(slotName) { 
    var adElem = document.createElement("img"); 
    var ad = "http://your-ad-here.com/great-ad-image.image"; 
    adElem.setAttribute("src", ad); 
    document.getElementById(slotName).appendChild(adElem); 
  } 
  Livefyre.require(['fyre.conv#qa'], function(Conv) { 
    new Conv({ 
      network: 'qa-0.fyre.co', 
        env: 'qa', 
        strings: { 
          'sponsored': 'Sponsored by: Livefyre' 
        } 
      }, [{ 
        app: 'main', 
        siteId: '291206', 
        articleId: '17', 
        el: 'livefyre-app-17', 
        ad: { 
          delay: 5, 
          frequency: 10, 
          delegate: function(data) { 
            var elem = document.createElement('div'); 
            elem.id = generateNextSlotName(); 
            return { 
              element: elem, 
              callback: function() { 
                insertSlot(elem.id); 
              } 
            }; 
          } 
        } 
      }], function (widget) { 
        // Initialize or Auth 
      }); 
    }); 
}()); 
</script>
```
