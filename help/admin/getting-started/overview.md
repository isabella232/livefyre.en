---

title: Get Started
description: Get started with Livefyre
seo-title: free text
seo-description: free text
short-title: free text
doc-type: article
author: name
index: yes
translate: yes
version:
private-feature-pack:
beta:
redirect:

---

# Get Started with Livefyre

Learn how to get started by building a fully working Livefyre App. Build off that App to handle basic authentication, social sharing, and event tracking.

When you get started with Livefyre, you will:

+ Perform the Implementation Process.
+ Decide your use case for implementing Livefyre Apps. 
    + For more information on what implementation options are available in Livefyre, see App Integration Types
+ Decide whether you want to use visualization Apps, conversation Apps, or both.
    + Visualization Apps are Apps that display content visually, including Carousel, Filmstrip, Media Wall, and Mosaic.
    + Conversation Apps are Apps that engage a site visitor in writing content that other site visitors can read, including Comments, Chat, and Reviews.
+ Decide if you will need authentication. 
    + If you already have a user management system (for example, Janrain, Giya), you can integrate it with Livefyre. 
    + If you don't, you can use Livefyre Identity, a built-in, lightweight user management system. 
    + For more about integrating authentication, see Identity: Identity Integration.

## Implementation Process

+ What to expect in implementing Livefyre Studio.
+ The length of time to implement Livefyre depends on your implementation and scope of work.

## Overview of Livefyre Network Architecture

Livefyre uses the following terms in discussing network architecture:

| Term    | Description                                                                                                                                                                                                                                                         |
| :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Network | The highest-level domain on which you plan to use Livefyre.                                                                                                                                                                                                         |
| Sites   | A subdomain or site section that is part of the network.                                                                                                                                                                                                            |
| Apps    | A rendering of content on your site. Content is displayed in Apps visually, using Visualization Apps (Mosaic, Carousel, Feature Card, etc.) or in text format, using Conversation Apps (Comments, Reviews, Chat, etc.). You can put one or more Apps on your sites. |
| Streams | Streams are filters that search social media and other sites to gather content automatically for moderation or direct publishing in an App.                                                                                                                         |
| Content | (for example, UGC, comments). What displays in the Apps. Content can be visual (for example, a photo or video), audio-only, or text.                                                                                                                                |

The following diagram shows the relationship between Network, Sites, Apps, and Content.

image

You have your own Livefyre instance which is your central dashboard for moderating content, managing users, and more. Contact your CSM for access to your Livefyre instance.

## Integration Steps

There are three main steps to integrating Livefyre:

1. App Integration
    + When you implement Livefyre, the style of implementation depends on your use case. For more on each implementation type, see App Integration Types.
1. Authentication Integration
   + You must integrate your existing user management system with Livefyre for conversation Apps and any other Apps that require end-user authentication on your site. If you do not currently use a user management tool, you can use Livefyre Identity. For more information about Livefyre Identity, what it is, and how to set it up, see Identity: Livefyre Identity..
1. Customization
    + Customization is optional, but most customers customize Apps to fit their brand.

## App Integration Types

When you implement Livefyre Apps, the style of implementation depends on your use case. The following table explains the features for the three available ways to create an App.

Table 1. CMS App Integration Type Overview
Type	Development Requirement	Features	Pros	Limitations
App Designer	Very Low	
Create JS embeds in Studio to add to pages without a developer
Limited Styling and Configurations available
Use case: Single Use Pages (event coverage, campaigns, hubs)
Able to get an App up and running in a short amount of time.
Configurations can be done by a non-technical member.
Easy on the fly changes to configurations
Must create an App using Livefyre Studio first
Not automated
Livefyre.js	Medium	
Integrate Apps into the JavaScript of your pages
Use case: Reusable templates (editorial content, product reviews)
Use the full suite of App customizations and configurations
Automates the process to dynamically instantiate Apps from within your CMS onto your pages
Need a developer up front.
SDK APIs	Advanced	
Retrieve your content from Livefyre to use for custom applications
Customize front-end beyond out supported offering
Use case: Data/Analytics integrations and custom front-end apps
Full power over the look and feel of App	
Requires development up front.
Higher level of dev effort to implement.

## Architecture

Learn Livefyre conventions and how Livefyre organizes content. This section provides an overview of the Livefyre Network Architecture.

+ Networks and Sites Overview
+ Understanding Networks
+ Understanding Sites
+ App Sequence Diagram

## Networks and Sites Overview

Livefyre organizes users and content by network and site. Every network may have one or more user accounts associated with it, and each network may include one or more Livefyre sites. A Livefyre site is an arbitrary grouping of Collections. One Collection maps to one article ID in your CMS.


## Understanding Networks

Customers with multiple domains can share user accounts across all domains, using a single Livefyre network. Customers that want to keep separate user accounts for different domains will require separate Livefyre networks.

Configuration settings can apply to sites, networks and Collections (referred to as conversation in the illustration above).

> [!NOTE]
> Some settings are available only at the network level (such as email notification preferences, email from address, and email custom logos). If you’d like these settings to be different for each domain, you must use multiple networks.

## Understanding Sites

A site is an arbitrary grouping of articles. The grouping is useful as it allows you to assign different moderators to different groups of content. Moderators and owners may be set up to moderate content and configure admin settings at either the network or the site level. 

If you would like some moderators to only see certain Collections, these Collections may be set up as a separate Livefyre site.

> [!NOTE]
> There is no limit to the number of sites you may have under your custom network.

## App Sequence Diagram

Whether you’re looking to implement custom function with Livefyre provided endpoints, or simply need to debug an issue, it helps to understand how the Livefyre app request/response flow works.


1. When your client hits your site, instantiate the Livefyre app with the Site ID and Article ID.
1. If you wish to authenticate the user (valuable for traffic evaluation, as well as site-protection), send Livefyre the site information, and User Profile token.
1. Send Livefyre the Site ID and Article ID to initialize the App.
    + Livefyre returns the initial content.
    + Send this content to the page, and display the App.
1. To update content displayed on the page, send Livefyre the latest Event ID from your page. If any new content is available, it will be returned.
1. Reload your page with new content, and repeat the process indefinitely.
1. If you allow users to post new content, trigger an event when new content is posted on your site to post the content to Livefyre. Livefyre will return an updated stream, which you can use to update your site.

## Device and Browser Support

A list of browsers and devices supported by the Livefyre App suite. Livefyre supports the following devices, operating systems and browsers.

| Browser     | Core Apps | Storify 2 | Studio | ModQ |
| :---------- | :-------: | :-------: | :----: | :--: |
| Chrome      |     Y     |     Y     |   Y    |  Y   |
| Edge        |     Y     |     Y     |   Y    |  Y   |
| IE 11       |     Y     |     Y     |   Y    |  Y   |
| Firefox 14+ |     Y     |     Y     |   Y    |  Y   |
| Safari 7+   |     Y     |     Y     |   Y    |  Y   |
 	 	 	 	 
| Device                                       | Core Apps | Storify 2 | Studio | ModQ    |
| :------------------------------------------- | :-------: | :-------: | :----: | :-----: |
| Android Browser 2.3+                         |  Limited  |  Limited  |  n/a   | Limited |
| Google Chrome on Android 4.1+                |  Limited  |  Limited  |  n/a   | Limited |
| iOS previous versions (iPhone 4S+ / iPad 2+) |  Limited  |  Limited  |  n/a   | Limited |
| iOS current versions (iPhone 4S+ / iPad 2+)  |     Y     |     Y     |  n/a   |    Y    |

> [!NOTE]
> While Livefyre will strive to maintain existing functionality, new products and features may not be entirely supported on browsers listed here with Limited support.

> [!IMPORTANT]
> Due to the end of support from Microsoft, Livefyre is not supported on Internet Explorer versions before Internet Explorer 11.

