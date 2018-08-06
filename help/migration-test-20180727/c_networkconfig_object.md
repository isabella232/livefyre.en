---
description: The NetworkConfig object is a JSON object that customizes the authentication system for network users.
seo-description: The NetworkConfig object is a JSON object that customizes the authentication system for network users.
seo-title: NetworkConfig Object
solution: Experience Manager
title: NetworkConfig Object
uuid: 259d7a54-2ee2-4546-a19d-bfa4e7ecaf80
index: y
internal: n
snippet: y
translate: y
---

# NetworkConfig Object

The `NetworkConfig` object is a JSON object containing the following parameters: 

| Parameter |Type |Description |
|---|---|---|
| * `authDelegate` * |Object (required) |Used to customize the authentication system for custom network users. |
| * `network` * |String (required) |A Livefyre-provided network name. For example: *yourname.fyre.co.* |
| * `attachmentDelegate` * |Object (optional) |Used to specify the types of media attachments visible in the App stream. For more information, see [Restricting Media](c_restrict_media.md#c_restrict_media).  |
| * `strings` * |Object (optional) |Used to customize text strings of the HTML elements in any of the Livefyre Core Apps. For more information, see [String Customizations](c_localize_strings.md#c_localize_strings).  |

