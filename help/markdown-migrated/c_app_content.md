---
description: Managing content across your Livefyre network.
seo-description: Managing content across your Livefyre network.
seo-title: App Content Tab
solution: Experience Manager
title: App Content Tab
---

# App Content Tab

On this page:
* [](#c_app_content/section_jvr_ntm_zz)
* [](#c_app_content/section_fw1_mtm_zz)
* [](#c_app_content/section_aqn_xqm_zz)
* [](#c_app_content/section_afl_vqm_zz)
* [](#c_app_content/section_ayz_tqm_zz)
* [](#c_app_content/section_xb4_mxr_rdb)
* [](#c_app_content/section_ls2_v4k_ybb)
* [](#c_app_content/section_emb_kqm_zz)
* [](#c_app_content/section_ojx_3qm_zz)
* [](#c_app_content/section_pyw_hqm_zz)

The App Content tab in your Library allows you to search and moderate content published across your Apps. The `uicontrol App Content` tab enables several search filters with wildcard search, to allow you to more quickly and easily define your search parameters.

Use the App Content tab to:

* Search for Content
* View Content History
* Moderate Content
* Add a Tag
* Feature Content
* Associate Content with Products from the Product Catalog
For more information on how to moderate content using the App Content tab, see [](c_moderate_content_using_app_content.md#c_moderate_content_using_app_content).

## Wildcard Search {#section_jvr_ntm_zz}

Livefyre search fields support wildcards, which allow you to add an asterisk ( * ) to words (or word fragments) to catch partial matches.

For example:

* ball returns only ball
* ball* returns ball and balloon
* *ball returns ball and football
* *ball* returns ball and uniball and snowballed
## Search for Content {#section_fw1_mtm_zz}

The App Content panel allows you to narrow your search using several different content filtering options.

![](images/PublishedState-1024x367.png)
Use the `uicontrol Quick Filters` pulldown to narrow returned content to `uicontrol All Content`, `uicontrol All Sidenotes`, `uicontrol Approved`, `uicontrol Approved &amp; Flagged`, `uicontrol Pending`, or `uicontrol Rights Requests` status. Then select a `uicontrol Filter by` option, and use the checkboxes or input fields available to narrow your search.

Use the pulldown menu to sort the content in the list by `uicontrol Newest`, `uicontrol Oldest`, `uicontrol Recently updated`, `uicontrol Most flags` or `uicontrol Most liked`.

## Filter by options {#section_aqn_xqm_zz}

Use the `uicontrol Filter by` bar to filter by the following options:

## Bozo Content {#section_afl_vqm_zz}

In Apps, `uicontrol Bozo` content is displayed only to the author of the content. This allows the user to believe their content has been approved, while hiding it from all other users and moderators.

>[!NOTE]
>
>Social content originating with SocialSync or Streams`uicontrol cannot` be set to Bozo.
You can Bozo content for the following reasons:

* Content identified as Spam by SAFE is automatically set to the Bozo state.
* All content from Banned Users is automatically set to Bozo.
* Content may be marked Bozo from Studio.
* Moderators may Bozo content directly in the stream.
## View Content History {#section_ayz_tqm_zz}

The content panel allows you to review the history of all content listed, including premoderation, spam filtering, post date, and any user flags or notes assigned to the item.

Use the tabs across the bottom of the content panel to view its history.

* `uicontrol More Info:` lists all activity on this content, including submission, editing, spam check, state change, and notes. The Livefyre Content ID and the user’s IP address is also displayed in this section.
* `uicontrol Replies:` lists a maximum of 6 replies. Click `uicontrol Show all replies` to display all replies to the post.
* `uicontrol Flags &amp; Reports:` lists all user flags, with the avatar of the user who flagged the content, and any Reports (notes that were added by the user when flagging the content).
* `uicontrol Add a note:` allows you to add a note, visible to other Admins or Moderators.
* `uicontrol Request Rights:` opens the `uicontrol New Rights Request` dialog, from which a Rights Request may be issued.
* `uicontrol Save as Asset:`opens the `uicontrol Advanced Options` dialog, which allows you to save the selected item to your Asset Library, Publish it to an App, or request reuse rights from its author.
![](images/PublishedMoreInfo-1024x462.png)
## Add a Tag to Content {#section_xb4_mxr_rdb}

Tagging content allows you to categorize and organize content for easy retrieval and style customization, or mark content as featured.

To add Tags, simply click the plus ( `uicontrol +`) icon under content. Enter a new tag, or select from a list of existing tags.

![](images/PublishedAddTag-1024x338.png)
## View Smart Tags {#section_ls2_v4k_ybb}

Livefyre uses Adobe Sensei image-recognition software to automatically tag content when you add it to the Library. The image recognition software has 135k classifiers, or tags, which include features (for example, cats, dogs, pyramids, Eiffel tower, Trump), categories (for example, travel, tourism, beauty), and aesthetic properties (for example, picture quality).

To view the smart tags on content:

1. In the Library, search for content from Twitter or Instagram.
1. Select one or more assets.
1. Add the assets to the Library.
1. Click one of the assets you added to the Library.
1. Click `uicontrol View Details` on the asset.
1. Click on the `uicontrol Tags` tab in the lower right panel
1. See the list of Smart Tags, arranged by category.
1. Delete tags that you do not want by clicking on the `uicontrol X` next to a tag.
## Searching for Images in All Assets {#section_zxf_hsf_wcb}

Once you have added the content to the library, you can search content by smart tags.

In the Library, under All Assets, you can search existing images by clicking on `uicontrol Show Filters` and then:
* Entering text to search in the search field
* Sorting by relevance
* Entering text in the `uicontrol Tags` field to search by Smart Tags. The Smart Tags ranking algorithm filters content using a smart tag confidence score, how new the content is, and how many stars a user gave the content.

## Featured Content {#section_emb_kqm_zz}

Select the default `uicontrol Featured` tag to mark the content as featured, and highlight it as important to your users. Once tagged, use custom styling options to customize Featured Content in your Apps.

## To Feature or Unfeature Content {#section_ojx_3qm_zz}

* From Studio, click the `uicontrol +` sign beside a piece of content, select the `uicontrol Featured` tag in the dropdown list, and click `uicontrol Enter` to Feature content. The tag will be saved and displayed beside the piece of content.
* To un-feature, click the `uicontrol x` on the `uicontrol Featured` tag displayed on the piece of content.
* From within a Comments, Live Blog or Reviews App, hover over the content you wish to feature, and click `uicontrol Feature`. To unfeature, simply hover over the content, and click `uicontrol Unfeature`.
>[!NOTE]
>
>Due to space constraints, Chat content may only be featured or unfeatured using Studio, and may not be featured from within the App itself.
## Editing Featured Content {#section_pyw_hqm_zz}

Most regular actions on content can be taken on Featured content, with the exception of the following:

* Featured content cannot be flagged.
* Users cannot edit their content after it has been Featured, although they can still delete it if they wish. Moderators can edit Featured content.
