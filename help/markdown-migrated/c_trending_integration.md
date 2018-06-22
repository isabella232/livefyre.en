---
description: Showcase the most active Collections on your Site or Network.
seo-description: Showcase the most active Collections on your Site or Network.
seo-title: Trending Integration
solution: Experience Manager
title: Trending Integration
---

# Trending Integration

Use Trending to showcase the Collections with the most recent activity in your Site or Network.

## Integration {#section_wtz_whb_c1b}

The quickest way to integrate with Trending is to use the built version hosted on Livefyre’s CDN.

First, add [ Livefyre.js ](https://github.com/Livefyre/Livefyre.js) to your page.

```
&lt;script src="//cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt; 

```
Then, position the element in which the App will appear.

```
&lt;div id="trending"&gt;&lt;/div&gt;
```
Finally, use `codeph  Livefyre.require` to construct the component.

```
&lt;script&gt; 
Livefyre.require([ 
 'streamhub-hot-collections#0' 
], function(Trending) { 
 var app = new Trending({ 
 el: document.getElementById("trending"), 
 network: 'livefyre.com' 
 }); 
 app.start(); 
}); 
&lt;/script&gt;
```
You now have a Trending App! See this all in action in [ this example ](http://codepen.io/gobengo/pen/GijEy).

## Configuration {#section_k5k_qhb_c1b}

`codeph  network`

The Network from which Collections will be pulled. (Required.)

```
var trending = new Trending({ 
 el: document.getElementById('trending'), 
 network: 'livefyre.com' 
});
```
`codeph  siteId`

Provide the Site ID to show Collections only from a single Site within your Network. (Optional.)

```
var trending = new Trending({ 
 el: document.getElementById('trending'), 
 network: 'livefyre.com', 
 siteId: 4 
});
```
`codeph  tag`

Provide a single Collection tag to show only Collections with that tag. (Optional.)

```
var trending = new Trending({ 
 el: document.getElementById('trending'), 
 network: 'livefyre.com', 
 siteId: 4, 
 tag: 'basketball' 
});
```
