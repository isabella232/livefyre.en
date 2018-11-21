---
description: Release Notes for the November 1, 2018 release.
seo-description: Release Notes for the November 1, 2018 release.
seo-title: November 1, 2018
solution: Experience Manager
title: November 1, 2018
uuid: 9d8b2bc0-6567-4db3-8695-df1a1f6a227a
index: y
internal: n
snippet: y
---

# November 1, 2018{#november}

Release Notes for the November 1, 2018 release.

## New Features {#section_syx_mdt_wcb}

The following new features were released in the production version of this release:

* Video Smart Tags

  Leverage state of the art computer vision technology, powered by Adobe Sensei, to automatically tag video content when you save it to the Library. Smart Tags help you manage UGC more effectively but also create super precise curation rules (streams) that collect content based on what's in the video, not just the text, saving you significant effort moderating unwanted content.

  Feature details:

    * Smart tags are automatically added to videos gained from social search, streams, and uploaded video files in the Library. View tags in the asset details for an individual video
    * Tags videos in .MP4, .MOV, and AVI formats
    * Tags videos up to 60 seconds or 50MB
    * Two categories of smart tags apply to videos: features ( animals, objects, places, etc) and actions (running, walking, singing, etc.)

  For more information see [](../c-smart-tags/c-smart-tags.md#c_smart_tags)

* Instagram Rate Limiting

  Instagram has changed the number of requests that any company using the Instagram API, including Livefyre, can make from 5,000 requests per hour per token to 200 requests an hour per token. This is known as *rate limiting*. For more information, see [](c_instagram_rate_limiting.md#c_instagram_rate_limiting).

* Audio Files in the Library

  You can now perform the following functions on audio files from the library panel:

    * Search
    * Preview
    * Import 
    * Filter by audio files
    * Drag and drop files into the designer

## Issues {#section_ehw_ndt_wcb}

No new issues were resolved in the production version of this release. See [](#c_rn/section_syx_mdt_wcb) section above.

## UAT Release {#section_EE91B0C9313E45C5B4CBD59CFBCCFCFE}

The issues in the following tables were resolved in the UAT version of this release.

<a id="section_5B8D1FD3834C47649CD5B93EEE53FACD"></a>

#### UAT Release
|  **Issue Type** | **Component** | **Release Note** |
|---|---|---|
|  Enhancement | GDPR | All data attributed to former customers within Analytics will be deleted. |
|  Bug | Library | Fixed an issue where a video uploaded to the Library, then viewed in asset detail did not display correctly. |
|  Bug | Mosaic | Fixed an issue where a Mosaic displayed the last piece of content from an Instagram carousel as a thumbnail, instead of a card.  |
|  Bug | Social Search | Fixed an issue where Instagram social searching didn't work as expected.  |

