---
description: You can use Livefyre Identity with GitHub Identity to allow users to use their GitHub logins to interact Apps on your site.
seo-description: You can use Livefyre Identity with GitHub Identity to allow users to use their GitHub logins to interact Apps on your site.
seo-title: Create a GitHub Identity App for Use with Livefyre Identity
title: Create a GitHub Identity App for Use with Livefyre Identity
uuid: 40c89c17-b82a-45da-b141-d3cde1feec2e
index: y
internal: n
snippet: y
translate: y
---

# Create a GitHub Identity App for Use with Livefyre Identity

To allow users to log in with their GitHub Identity credentials, Livefyre requires the following GitHub Identity Information:

* Client ID (Private Key)
* Client Secret (Password)
To create an GitHub Identity App for use with Livefyre Identity:

1. Create or sign in to a GitHub account at [](https://github.com/settings/developers).
1. Register a new or select an existing app for use with Livefyre Identity.
1. Enter all information on the form. Enter the ** `Authorization callback URL` **, using your network name instead of `{network-name}: {network-name}: https://identy.livefyre.com/{network-name}.fyre.co/api/v.1.0/public/profile/social/complete/github_fyre`.
1. In ** `Livefyre Integration Settings Livefyre Identity GitHub` **, switch the ** `Enable GitHub Login` ** toggle to ** `On` **.
1. Enter the GitHub Client ID and GitHub Client Secret.
1. Click ** `Save Settings` **.
When complete, GitHub Identity’s app details page will list the App’s Client ID (Consumer Key) and Client Secret (Consumer Secret) for use in Studio’s Integration Settings page.
