---
description: You can whitelist your video domain using .
seo-description: You can whitelist your video domain using .
seo-title: userPrivacyVideoWhitelist
solution: Experience Manager
title: userPrivacyVideoWhitelist
uuid: c4468865-023a-42c5-aaa7-c62c551656c6
index: y
internal: n
snippet: y
translate: y
---

# userPrivacyVideoWhitelist

You can whitelist your video domain using .

If you use your own custom videos and players as part of the videos that display in a Livefyre visualization App, you can whitelist your video domain. Whitelisting your video domain removes the video mask for your custom videos and players.

>[!NOTE]
>
>Use specific paths to ensure only the videos that are safe are whitelisted. If you put a broad path (for example, sampledomain.com), you may whitelist unsafe videos.

Add `userPrivacyVideoWhitelist` after `userPrivacyOptOut`. You can add all the Livefyre privacy flags all at once as part of one Livefyre object.

`userPrivacyVideoWhitelist` only applies to content that is not embedded from social media.

In the following example, videos displaying in Apps with the `sampledomain.com/cdn/videos` path are whitelisted:

```
userPrivacyVideoWhitelist: ["sampledomain.com/cdn/videos"]
```

