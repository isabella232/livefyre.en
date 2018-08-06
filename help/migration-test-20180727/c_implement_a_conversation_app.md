---
seo-title: Implement a Conversation App
solution: Experience Manager
title: Implement a Conversation App
uuid: a2889706-5062-4545-8516-ca941bbff7fc
index: y
internal: n
snippet: y
translate: y
---

# Implement a Conversation App

## Implement a Conversation App {#concept_zvy_c3c_tbb}You implement all conversation Apps using the same basic procedure. To implement a conversation App:

1. Embed a core App. For information on how to embed a core App, see [](c_using_livefyre.js_to_create_customize_and_use_apps_on_your_site.md#c_using_livefyre.js_to_create_customize_and_use_apps_on_your_site).
1. Create authentication tokens to use to authenticate users for an App using App Objects. Most Apps use the following objects:
    * NetworkConfig Object, see [](c_networkconfig_object.md#c_networkconfig_object)
    * ConvConfig Object, see [](c_convconfig_object.md#c_convconfig_object)
    * CollectionMeta Object, see [](c_collectionmeta_object.md#c_collectionmeta_object)

1. Add an Event Handler. See [](c_adding_an_event_handler.md#c_adding_an_event_handler).
1. Build Server-side Tokens.
1. Some Apps require additional, or slightly different implementations. For examples and App-specific implementation details, see the following App-specific integration information:
    * Comments, see [](#concept_twr_xyd_tbb)
    * Chat, see [](c_chat_integration.md#c_chat_integration)
    * Reviews, see [](c_reviews_integration.md#c_reviews_integration)
    * Liveblog, see [](c_live_blog_integration.md#c_live_blog_integration)
    * Sidenotes, see [](r_sidenotes_integration.md#r_sidenotes_integration)

