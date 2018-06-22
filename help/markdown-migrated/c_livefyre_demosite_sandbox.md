---
description: Using the Demosite to evaluate the Livefyre product suite.
seo-description: Using the Demosite to evaluate the Livefyre product suite.
seo-title: Livefyre Demosite Sandbox
title: Livefyre Demosite Sandbox
---

# Livefyre Demosite Sandbox

>[!NOTE] {importance="high"}
>
>PLEASE NOTE: Livefyre demosites are created and intended for demonstration purposes ONLY! Please do not create Collections with the purpose of integrating or producing content you wish to have in your production environments. For more information, please contact your Livefyre Sales Representative or Livefyre Solutions Engineer.
The Livefyre demosite sandbox provides you with a working introduction to the Livefyre product suite, and includes examples of both Core and SDK Apps. This sandbox allows you to explore the structure of these App integrations, and provides access to the Collections used to power these Apps. You may also manipulate the Curate rules used to power these Collections. Use this site to develop a greater understanding of the product offering, and learn how to customize Collections and the Livefyre Apps.

>[!NOTE]
>
>While the sandbox does not allow you to customize styles, layout, or other CSS, you may load the provided example code onto your own servers, and customize at will.
Your sandbox includes the following pages:

* Core Apps: Combines Comments with Sidenotes and a Poll to demonstrate how Core Apps are embedded.
* Live Blog: Provides a sample of the Live Blog App, with Sidenotes embedded for the image.
* Reviews: Provides a demonstration of the Reviews App.
* Curate Apps: Uses a Media Wall to demonstrate the use of Curate to power an SDK App.
* Social Hub: Combines Maps, Trending, and a Media Wall with an implementation of the Featured Items API to illustrate how to combine multiple Apps on the page.
* APIs: Links to the HTTP APIs page on the Livefyre Answers site.
* Docs: Links to the developer docs on the Livefyre Answers site.
* Login: Allows you to log into the demosite, and create new users.
## Core Apps {#section_srs_sth_xz}

The Core Apps tab provides examples of the Comments, Sidenotes, and Polls Apps.

Core Apps include Comments, Chat, Live Blog, Sidenotes, and Reviews. These Apps rely upon fyre.conv for integration, and differ from SDK apps in some of their integration options. Your sandbox provides an implementation of the Comments App, and showcases Sidenotes to demonstrate how users may annotate content in an article.

## Creating Collections {#section_d25_4th_xz}

Both Core Apps and SDK Apps are powered by Collections.

While you may create Collections from within Studio, you may also use your CMS to create new Collections on the fly as you publish new content. To create new Collections on the fly, your CMS must publish the markup and script to instantiate the App with the unique identifier of the article being published. This script must include a CollectionMeta token, signed server-side with your unique Site API Key, in order to securely create Collections.

>[!NOTE]
>
>Even though this is a server touchpoint, this Collection Metadata token may be cached in perpetuity, and only needs to be regenerated when the data within it changes.
## Live Blog {#section_mct_2th_xz}

The Live Blog tab provides a demo sample of the Live Blog App, allowing users to read and follow blogs. The page also provides a demonstration of Sidenotes, allowing users to post comments to the image.

## Reviews {#section_xvl_dth_xz}

The Reviews page provides a simple demo of the Reviews App, allowing users to click to select the number of Star ratings, and use the text fields to provide a title and content for their review.

Users may also upload images, reply to reviews, and share to their social networks.

## Curate Apps {#section_shf_cth_xz}

The Curate Apps tab provides an example of a Media Wall, powered by Curate Rules.

Use Livefyre Studio to create Curate Collections to power your Apps. Use Curate Rules to automatically aggregate and power your real-time Apps, bringing social buzz from other sources back onto your site. Curate Rules allow you to create rules by which social content from Twitter, Facebook, Instagram and any RSS feed (like YouTube, Pinterest, or WordPress blog feeds) may be automatically pulled into your Apps. Curate Search allows you to search for targeted social content, and add selected content to your Apps.

The Media Wall is built on the Livefyre JavaScript SDK. Your sandbox example uses Curate to power a Collection which streams live images and other content, aggregated from Instagram, Twitter, Vine and other sites, into a real-time social wall, visualizing all activity surrounding an event.

## Social Hub {#section_a32_zsh_xz}

The Social Hub page combines several SDK Apps on the page (Maps, Trending, and Media Wall), and incorporates an example use case of the Featured API. This page demonstrates both the use of multiple Apps to present a single story, and the use of Livefyre.js to authenticate across several Apps on a single page.

SDK Apps are implemented using Livefyre.require and the Livefyre SDK. Livefyre.require is a custom JavaScript module loader, which can be used to load most packages published by Livefyre and presents a convenient and intuitive integration path. The Livefyre SDKs provide a thin wrapper around the most common APIs, and enable more rapid integration with our featured App types.

## Maps {#section_ubl_ysh_xz}

Maps pulls geotagged content, based on Curate Rules, and displays it on an interactive world map. Users may click the map to reposition and zoom in on selected content, and may click content groups to display them in a Gallery console. Maps are powered by Leaflet.js and can be further customized using the Leaflet.js options ([http://leafletjs.com/reference.html#map-options](http://leafletjs.com/reference.html#map-options)).

## Media Wall {#section_rbd_xsh_xz}

Media Walls generate a gridded display of user generated content. Content may also be loaded using Curate Collections.

## Trending {#section_xrj_wsh_xz}

Use the Trending App to provide a real-time display of the most active Collections on your site or network. Users may click one of the Collections displayed to navigate to the App displaying that Collection on your site.

## Featured Items {#section_lnn_vsh_xz}

Use the [Featured APIs](http://livefyre-devhub-production.herokuapp.com/developers/api-reference/#feature) to feature selected content in your Apps, allowing you to call attention to content you consider to be most valuable.

## Login {#section_bbh_5sh_xz}

The Demosite provides a simplified login experience, allowing you to comment within the Core Apps and access Studio from within the demo site. This login is an authenticationless stand-in for true SSO, and is not meant to demonstrate the Livefyre auth process.

Your Livefyre Technical Integration Manager will create your account, and send you the link to the site. Use the Login pulldown menu to log in, log out, or create new users. You may also use the Login pulldown to create new users, and give them access to the demosite. Use this feature to test multi-user posts, replies, reviews, and other Livefyre App functionality.

>[!NOTE]
>
>Your Livefyre Demosite has a simple mockup for SSO authentication. Your own SSO or Livefyre Enterprise Profiles would be used in your production environment. The Admin user account provides access to Livefyre Studio where you can create additional users for testing purposes during your trial period.
