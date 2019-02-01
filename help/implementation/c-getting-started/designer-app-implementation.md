---
description: Use Bootstrap and Stream API with Livefyre Apps.
seo-description: Use Bootstrap and Stream API with Livefyre Apps.
seo-title: App Implementation
solution: Experience Manager
title: App Implementation
uuid: 

---
## App Implementation {#appimplementation}

Use Case: As a customer, I want to integrate Livefyre into my 3rd party CMS using the Livefyre.js method.

There are three ways to implement Livefyre in to a custom AEM component or other CMS' like WordPress, Sitecore, or DemandWare: Designer App Implementation, API, Implementation, and Third Party Authentication Integration.

## Designer App Implementation {#designerapp}

What: Simplest and fastest way of integrating a Livefyre App. You can design, configure, and generate a customized Javascript embed code to integrate a Liveyfre App on a page in minutes.
How: Create, Preview, Publish, and Embed a Livefyre App
Example: https://codepen.io/dharafyre/pen/bvGrLo

### Livefyre.js Implementation {#livefyrejsimp}

What: Livefyre.js is the core library that powers Apps and Auth on a site. It defines the global window.Livefyre object and a single public method, Livefyre.require, which can be used to load other Livefyre JavaScript libraries that help with embedding Livefyre Apps and integrating with third party User Auth platforms.

How:
Create a Collection Using the CollectionMeta Token
Integrate Apps into third part CMS using App Integrations.
Example:

Comments App: [https://codepen.io/dharafyre/pen/oYoJdP](https://codepen.io/dharafyre/pen/oYoJdP)
Reviews App: [https://codepen.io/dharafyre/pen/GXgvvd](https://codepen.io/dharafyre/pen/GXgvvd)
Media Wall: [https://codepen.io/dharafyre/pen/dNMPvM](https://codepen.io/dharafyre/pen/dNMPvM)
For advanced customizations using the SDK, please see StreamHub SDKs.

## API Implementation {#apiimplementation}

For creating customized experiences and data visualizations, Livefyre Apps can be created from scratch by consuming Livefyre and social data using the Bootstrap and Stream API.

## Third Party Authentication Integration {#thirdpartyauth}

For Livefyre Apps requiring authentication, please see Identity Integration for third party authentication platforms.

## Customer Examples {#customerexamples}

The following customers implemented Livefyre with Third Party CMS Integrations:

PGA Tour Media Wall
TimeOut
