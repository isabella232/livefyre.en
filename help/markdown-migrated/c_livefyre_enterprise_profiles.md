---
description: Work with Livefyre’s all-in-one user management system.
seo-description: Work with Livefyre’s all-in-one user management system.
seo-title: Livefyre Enterprise Profiles
title: Livefyre Enterprise Profiles
---

# Livefyre Enterprise Profiles

Skip this section if you use a custom or third-party user management system.

Livefyre Enterprise Profiles customers may use these instructions to integrate with Livefyre JS Auth, and enable your community to more easily authenticate with Livefyre Apps.

You can see an example integration in action [ here ](http://codepen.io/zjj/pen/frhLv).

If you think Livefyre Enterprise Profiles may be a good fit for your community, please contact your Livefyre Account Manager.

## Step 1: Add Livefyre.js {#section_n4k_g3s_p1b}

If you have never done so, add Livefyre.js to the &lt;head&gt; element of your webpage or website template. Livefyre.js is a small base library that other Livefyre components also use. Livefyre.js provides a global window.Livefyre variable to your pages, and Livefyre.require, which can be used to load other Livefyre packages on demand.

```
&lt;script src="//cdn.livefyre.com/Livefyre.js"&gt;&lt;/script&gt;
```
## Step 2: Add customprofile.js {#section_aqr_h3s_p1b}

Add the Livefyre Enterprise Profiles JavaScript library (a file specific to your installation that ends with customprofile.js) to the &lt;head&gt; element of your HTML document.

For example:

```
&lt;script src="//client-solutions.ep.livefyre.com/media/Y2xpZW50LXNvbHV0aW9ucy5lcC5saXZlZnlyZS5jb20=/javascripts/customprofiles.js"&gt;&lt;/script&gt;
```
>[!NOTE]
>
>Contact your Livefyre Technical Account Manager to acquire your specific customprofile.js URL.
>
>
## Step 3: Register an LFEP Auth Delegate {#section_eqb_t1h_21b}

Livefyre.js Auth is Livefyre’s package for ensuring that all the social components on your page can discover a single auth integration. Auth must be provided an AuthDelegate object that knows how to perform authentication actions, like login and logout. Livefyre also provides an lfep-auth-delegate package that will make an appropriate auth delegate for you.

To tell Auth to delegate these actions to LFEP, add the following to your webpage after Livefyre.js:

```
Livefyre.require(['auth', 'lfep-auth-delegate#0'],function (auth, LFEPAuthDelegate) { // create an LFEP Auth Delegate var authDelegate = new LFEPAuthDelegate({ engageOpts: { app: 'example.auth.fyre.co' } }); // Delegate AppKit Auth actions to LFEP auth.delegate(authDelegate);});
```
>[!NOTE]
>
>LFEP creates a Janrain Engage App on your behalf that allows visitors on your site to use social authentication to sign in and interact with content.***{Your Janrain Engage App Name}***will be provided to you by your Livefyre Technical Account Manager.
## Step 4: Add your domain to the Janrain whitelist {#section_rrh_s1h_21b}

To complete your Enterprise Profiles integration, you must add your Livefyre Enterprise Profiles domain name (for example: &lt;site&gt;.ep.livefyre.com) to the Janrain Application Settings &gt; Domain Whitelist. For more information, see the [ Janrain documentation ](http://developers.janrain.com/reference/janrain-dashboard/social-login/).

## Step 5: Add Social Networks {#section_ftq_wxg_21b}

To take advantage of social login from providers like Twitter and Facebook, you must add your social network app keys through the Janrain Dashboard. Once this configuration is complete, you can add them to your sign-in modal.

Your selected social network providers must be set up with app API tokens and keys for each network.

1. Go to the Providers area in the Janrain Engage Dashboard.
1. Click on the gear button for each social network to enter the credentials for that provider. (The gray gears will turn lime green once each has been configured.)
1. When you’ve completed configurations, go to Widgets &amp; SDKs &gt; Sign-ins and add your configured providers to the modal.
