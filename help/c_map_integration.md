---
description: Plot user content to an interactive map.
seo-description: Plot user content to an interactive map.
seo-title: Map
solution: Experience Manager
title: Map
uuid: bd36abbb-a7c7-41cf-b289-c5ffcd6f40d5
index: y
internal: n
snippet: y
translate: y
---

# Map

Plot user content to an interactive map.

On this page:

* [](#c_map_integration/section_w2m_db2_d1b) 
* [](#c_map_integration/section_jc5_gxb_c1b)

Map allows you to stream geotagged content onto a world map, allowing you to locate the social buzz around breaking news or a live event. All applicable content will be displayed, including text, comments, photos, and Tweets.

>[!NOTE]
>
>Maps are powered by [©OpenStreetMap](http://www.openstreetmap.org/copyright), which provides the data Livefyre uses to render its Maps.

## Integration {#section_w2m_db2_d1b}

The quickest way to use Map is to use the built version hosted on Livefyre’s CDN.

First, add [Livefyre.js](https://github.com/Livefyre/Livefyre.js) to your page.

```
<script src="http://cdn.livefyre.com/Livefyre.js"></script> 

```

Then, position the element in which the Map App will appear.

```
<div id="map" style="height: 500px;"></div>
```

Finally, use Livefyre.require to construct the Map, and get a Collection to pipe in from streamhub-sdk. Keep in mind that Map can show only Content with geotagged metadata. Twitter and Instagram Curate support this feature. To ensure best performance, include a geolocation filter on all of your Curate Rules for the Collection.

```
<script> 
Livefyre.require(['streamhub-map#1', 'streamhub-sdk#2'], 
function (Map, SDK) { 
    var map = new Map({ 
        el: document.getElementById('map') 
    }); 
    var collection = new SDK.Collection({ 
        network: 'strategy-prod.fyre.co', 
        siteId: 340628, 
        articleId: 'custom-1389845009515' 
    }); 
    collection.pipe(map); 
}); 
</script>
```

Check out this [live example](http://codepen.io/cheung31/pen/wkmbF).

## Configuration {#section_jc5_gxb_c1b}

`initial`

The initial number of items to load from the Collection and display on the map. After this number are loaded, users may click a button to show more. (Optional. Defaults to 50.)

```
var map = new Map({ 
    el: document.getElementById('map'), 
    initial: 100 
});
```

`leafletMapOptions`

Options to pass to the underlying [Leaflet](http://leafletjs.com/) map, which Map uses for rendering. Use this option to set [Leaflet Map Options](http://leafletjs.com/reference.html#map-options), including the initial centerpoint of the map, and initial and maximum zoom levels. (Optional.)

```
var map = new Map({ 
    el: document.getElementById('map'), 
    leafletMapOptions: { 
        center: [37.774, -122.4], 
        zoom: 15 
    } 
});
```

