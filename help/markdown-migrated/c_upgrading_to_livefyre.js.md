---
description: Upgrading existing implementations from livefyre.js to Livefyre.js.
seo-description: Upgrading existing implementations from livefyre.js to Livefyre.js.
seo-title: Upgrading to Livefyre.js
solution: Experience Manager
title: Upgrading to Livefyre.js
---

# Upgrading to Livefyre.js

On this page:

* [](#c_upgrading_to_livefyre.js/section_vsw_fhh_xz)
* [](#c_upgrading_to_livefyre.js/section_zt3_1hh_xz)
* [](#c_upgrading_to_livefyre.js/section_fkr_sgh_xz)
* [](#c_upgrading_to_livefyre.js/section_tcb_m2h_xz)
* [](#c_upgrading_to_livefyre.js/section_mdy_k2h_xz)
* [](#c_upgrading_to_livefyre.js/section_uv1_jch_xz)
* [](#c_upgrading_to_livefyre.js/section_as5_fyg_xz)
* [](#c_upgrading_to_livefyre.js/section_g5b_fyg_xz)
* [](#c_upgrading_to_livefyre.js/section_glz_cyg_xz)
`codeph  Livefyre.js`, and its public method `codeph  Livefyre.require`, provide a new way to implement Livefyre in a modular fashion. By leveraging the JavaScript Module Loader ( [ http://requirejs.org/ ](http://requirejs.org/)), Livefyre can import any of our most popular Apps with a simple, human readable, version pinned, instance of the App.

Using `codeph  Livefyre.require` also simplifies the auth integration process. Using `codeph  Livefyre.require`to load auth allows you to create a single auth for each page on your site. Once enabled, all Apps on the page will share this common authentication.

* Check your Livefyre Library Status
* Advantages
* Implementation
* Examples
## Check your Livefyre Library Status {#section_vsw_fhh_xz}

Livefyre offers a simple bookmarklet test, allowing you to quickly and easily check your current implementation status. Drag this button to your bookmark bar to enable this functionality.

Livefyre.js Status

Once installed, `codeph  Livefyre.js` Status will appear as a bookmark in your browser.

To test your Livefyre library status:

* Go to a page where Livefyre is integrated (Comments, Reviews, Maps, or other Livefyre Apps).
* Click on the bookmarklet.
* A modal will appear displaying the status of your Livefyre library.
If you find that your Livefyre Apps are using the old livefyre.js, please upgrade to the new Livefyre.js using the following upgrade guide.

## Advantages {#section_zt3_1hh_xz}

Adding Livefyre.js to your site will not break existing implementations, and can be done slowly, over time, and page by page. Moving toward this implementation provides several advantages, including more streamlined auth integration, faster page loads, and an easier App implementation process.

Upgrading to `codeph  Livefyre.js` and `codeph  Livefyre.require` also allows for version pinning, greater code clarity, and a lower integration bar for multiple Apps on the page.

* **Version Pinning:**Semantic Versioning allows you to pin to major, minor, or patch releases, allowing you to decide when you’re going to upgrade your Livefyre code. This preserves any customizations you might have made, as well as allowing you to avoid unnecessary upgrades.
* **Code Clarity:**The `codeph  Livefyre.require` model follows a much more modular design than the previous model, with clearly designated class structure.
* **App Access:**All new Livefyre Apps will use `codeph  Livefyre.js`. Many existing Apps, including Media Wall with Auth, Maps, Feed, Sidenotes, and Trending, already require the new `codeph  Livefyre.js`.
* **Ease of App Installation:**With `codeph  Livefyre.require` installed, adding new applications to the page is as easy as including them in the initial require load.
## More lightweight authentication, with easier integration {#section_fkr_sgh_xz}

Using the new Livefyre.js (rather than the older system of livefyre.js) allows you to authenticate across multiple Apps on a page with only a single instance of auth. Livefyre.js Auth provides a centralized authentication integration for all Livefyre Apps across your site, allowing you to add authentication for all Apps on a page with a single call.

Add Auth to your site’s template (ie. any **global scope**) will allow it to cascade to all pages on your site. Once your users have signed in, Auth will automatically broadcast the current user’s information to all Apps on the page.

## Faster page loads, with an increase in performance {#section_tcb_m2h_xz}

Adding the `codeph  Livefyre.js` script to your page will embed a very small (~1 Kb) file called the `codeph  Livefyre.js` scout, that will load the latest version of `codeph  Livefyre.js` over the protocol with which your webpage has been accessed (HTTP or HTTPS).

`codeph  Livefyre.js` polls for newer versions less frequently than the previous livefyre.js.

Because `codeph  Livefyre.require` pulls in only needed Apps (and not all Core Apps), file footprints shrink dramatically. By including only the Livefyre.js file, you’ll be able to hand pick Apps that will be downloaded and useable on the page.

## Implementation {#section_mdy_k2h_xz}

`codeph  Livefyre.require`is a structural change only. Previous Apps, such as Comments and Media Walls are still available. The only difference is they will now be loaded using the Livefyre.require method.

Using `codeph  Livefyre.js`, all Apps are loaded onto the page using the following pattern:

```
Livefyre.require([‘module_name1#version’, ‘module_name2#version’] function(AppName1, AppName2) { 
 new AppName1(args); 
 new AppName2(args); 
});
```
## Examples {#section_uv1_jch_xz}

These examples are included in this GitHub pull request: [ https://github.com/soldnermike/require-upgrade/pull/1 ](https://github.com/soldnermike/require-upgrade/pull/1).

## Core Apps (Comments/Blog/Chat) {#section_as5_fyg_xz}

To add a Core App to your page, add `codeph  Livefyre.js` to the head element of the page:

```
&lt;head&gt; 
 &lt;script src='//cdn.livefyre.com/Livefyre.js'&gt;&lt;/script&gt; 
&lt;/head&gt; 
 
// Then use Livefyre.require to add the App: 
Livefyre.require(['fyre.conv#3'], function(Conv) { 
 new Conv(networkConfig, [convConfig], function(widget) {}); 
});
```
For an example, see [ http://codepen.io/soldnermike/pen/PwqzpJ ](http://codepen.io/soldnermike/pen/PwqzpJ).

## SDK Apps {#section_g5b_fyg_xz}

Livefyre SDK Apps have used `codeph  Livefyre.require` since their inception. Their migration will not be described here.

## Authentication {#section_glz_cyg_xz}

Using `codeph  Livefyre.require`allows you to add auth a single time in a single global space. Once on the page, all Apps will use the same code to authenticate.

To add authentication to your page, add `codeph  Livefyre.js` to the head element of the page:

```
&lt;head&gt; 
 &lt;script src='//cdn.livefyre.com/Livefyre.js'&gt;&lt;/script&gt; 
&lt;/head&gt; 
 
// Then use Livefyre.require to add auth to the page: 
Livefyre.require(['auth'], function (auth) { 
 // Do authy things... }); 
 
//Finally, register the authDelegate: 
Livefyre.require(['auth'], function (auth) { 
 auth.delegate({ 
 login: function (errback) { 
 errback(null, { livefyre: '&lt;userAuthToken&gt;' }); 
 } 
 }); 
});
```
For an example, see [ http://codepen.io/soldnermike/pen/QwbEpB ](http://codepen.io/soldnermike/pen/QwbEpB).

