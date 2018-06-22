---
description: Build the ping so your page pings Livefyre when users update their profile.
seo-description: Build the ping so your page pings Livefyre when users update their profile.
seo-title: Build the Ping
solution: Experience Manager
title: Build the Ping
---

# Build the Ping

When Livefyre receives an update notification with the `codeph networkName` and `codeph user_id`, the system will send a Pull request to your Ping for Pull URL.

>[!NOTE]
>
>403/Not Authorized in response to your Ping indicates an invalid`codeph lftoken` appended to the Ping request. Please ensure that the `codeph lftoken` is for a `codeph user_id` with network owner privileges or the system user. If you are using Livefyre libraries, use the `codeph buildLivefyreToken` method to generate a valid system token for the request.
>1. Add code to your page that pings Livefyre when users update their profile. Construct the URL this way:
>   ```
>   POSThttps://{networkName}.quill.fyre.co/api/v3.0/user/{user_id}/refresh?lftoken={token}
>   ```
>* `uicontrol networkName:` Your Livefyre provided network name.
>* `uicontrol user_id:` Your user’s ID.
>* `uicontrol token:` Valid system token.
>   
>   
>1. Pull the request structure.
>   
>   
