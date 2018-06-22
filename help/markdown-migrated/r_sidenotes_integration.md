---
---

<a id="section_qyc_cpv_sy"></a>

As a general rule, if your Core Application integration is complete, the code written to generate the `codeph  collectionMeta` object may be reused for Sidenotes.

You can also reuse your existing `codeph  auth` delegates by supplying an `codeph  auth` delegate created with `codeph  fyre.conv` to Sidenotes in the (optional) `codeph  authDelegate` field.

>[!NOTE]
>
>Sidenotes allows you to include`codeph  network`, `codeph  siteId`, and `codeph  articleId` in a single object, rather than passing them separately in other parts of the constructor.
```
&lt;!DOCTYPE html&gt; 
&lt;html&gt; 
&lt;head&gt; 
&lt;!-- First add Livefyre.js to the page --&gt; 
&lt;script src="http://cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt; 
&lt;/head&gt; 
&lt;body&gt; 
&lt;script type="text/javascript"&gt; 
var convConfig = { 
 network: 'client-solutions.fyre.co', 
 selectors:'span.lyrics-sidenote', 
 siteId: '356373', 
 articleId: 'sidenotes-sample', 
 collectionMeta: 'eyJhbGciOiAiSFMyNTYiLCAidHlwIjogIkpXVCJ9.eyJ1cmwiOiAiaHR0cDovL3d3dy5zaWRlbm90ZXMtZGVtby5jb20vbHlyaWNzIiwgInNpdGVJZCI6ICIzMDQwNTkiLCAidHlwZSI6ICJzaWRlbm90ZXMiLCAiYXJ0aWNsZUlkIjogInNpZGVub3Rlc19zYW1wbGUiLCAidGl0bGUiOiAiQ2xpZW50IFNvbHV0aW9ucyBTaWRlbm90ZXMifQ.2gxnsM0TS8dfp-Jokb5uW1kuMl-DqIlqfJSCBwJgf1k' 
}; 
 
Livefyre.require(['sidenotes#1', 'auth'], function (Sidenotes, Auth) { 
 new Sidenotes(convConfig); 
 Auth.delegate({ 
 login: function (callback) { 
 callback(null,{livefyre:'&lt;userauthtoken&gt;'}); 
 } 
 }); 
 }); 
&lt;/script&gt; 
&lt;/body&gt; 
&lt;/html&gt;
```
As noted in the Building `codeph  collectionMeta` section, `codeph  collectionMeta` is an encoded JSON object. In the example above, the JSON object takes the following format before it’s JWT encoded.

```
{ 
"title":"Client Solutions Sidenotes", 
"url":"http:\/\/www.livefyre.com\/sidenotes", 
"articleId":"sidenotes_sample", 
"siteId":"304059", 
"type":"sidenotes" 
}
```
For more information, please see the `codeph  collectionMeta` token.

**Mobile Setup**

Sidenotes has been optimized for use in mobile devices. For best results with mobile versions of your Livefyre App, set the user-scalable option to no. For example:

```
&lt;meta name="viewport" content="width=device-width, user-scalable=no"&gt;
```
