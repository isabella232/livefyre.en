---
description: Create a new Collection by creating a collectionMeta token that is passed to Livefyre.
seo-description: Create a new Collection by creating a collectionMeta token that is passed to Livefyre.
seo-title: Create a Collection Using the CollectionMeta Token
solution: Experience Manager
title: Create a Collection Using the CollectionMeta Token
uuid: 831a874e-4c9f-4bc0-8d6b-ca358eddd99a
index: y
internal: n
snippet: y
translate: y
---

# Create a Collection Using the CollectionMeta Token


>1. Create the collectionMeta token.
>1. Create the checksum.
>   The checksum is required if you wish to notify Livefyre of any changes that you’ve made to your Collection. Livefyre will update your Collection only if the checksum provided is different than the previously sent checksum. Creating a checksum is just like creating a collectionMeta token but instead of calling buildCollectionMetaToken you call buildChecksum.
>
