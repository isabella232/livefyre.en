---
description: You can choose various sorting options depending on the App and what you want site visitors to be able to do.
seo-description: You can choose various sorting options depending on the App and what you want site visitors to be able to do.
seo-title: Sort Features
solution: Experience Manager
title: Sort Features
uuid: 50a3d1a7-f61f-4748-86a1-042f797a14a2
index: y
internal: n
snippet: y
translate: y
---

# Sort Features

## Sort Features {#c_sort_features}You can choose various sorting options depending on the App and what you want site visitors to be able to do.On this page:

* [](#c_sort_features/section_elc_hfs_d1b)
* [](#c_sort_features/section_grr_hfs_d1b)
* [](#c_sort_features/section_t4s_hfs_d1b)
* [](#c_sort_features/section_cft_hfs_d1b)
* [](#c_hot_threads)
<!-- c_sort_features.dita --> 
## Sort by Rating {#section_elc_hfs_d1b}

This feature is only available for Reviews. Sort content by number of stars or other quality metric rating.
Apps that use this feature:

* [Reviews](c_reviews_app.md#c_reviews_app)

## Sort by Helpfulness {#section_grr_hfs_d1b}

This feature is only available for Reviews. Sort content by the number of site visitors that found a piece of content helpful.
Apps that use this feature:

* [Reviews](c_reviews_app.md#c_reviews_app)

## Sort by Newest to Oldest, First to Last {#section_t4s_hfs_d1b}

For the Comments App, you can choose to allow users to sort from the most recently published content to least recently published content.
In Storify 2, site visitors can sort from the first post to the last post or from the last post to the first post. Storify 2 posts appear in the order a moderator decides, not based on published time.
Apps that use this feature:

* [Chat](c_chat_app.md#c_chat_app)
* [Comments](c_comments_app.md#c_comments_app)
* [Reviews](c_reviews_app.md#c_reviews_app)
* [Storify 2](c_storify2.md#c_storify2)

## Top Comments {#section_cft_hfs_d1b}

Top Comments lists the 25 most liked comments in the conversation. The ** `Top Comments` ** view displays the 25 most liked comments in the Collection. If an original post receives the most likes, the post, but not its replies, will be listed. If a reply receives the most likes, its immediate parent, up to the top level post, will also be displayed. This list is not real-time, and will update only when the page is refreshed or another sort view ( ** `Newest` ** or ** `Oldest` **) is selected.
If a user posts a comment from the comment editor while viewing the ** `Top Comments` ** view, the user will be switched back to the ** `Newest` ** view. If a user likes or replies to one of the Top Comments, it will stream into the ** `Top Comments` ** view for the user to see.
To optimize for performance, Livefyre caches data for up to 2 minutes. There may be a slight lag in the most recent likes that appear.
If there are no comments in the Collection with likes, users will see the message ** `There are not enough likes yet` **, and a link to ** `See what’s new` **.

>[!NOTE]
>
>Top Comments and Hot Threads may not be included in the same Collection.

For information on enabling the Top Comments view, please see ** `Studio > Network Settings` **.
Apps that use this feature:

* [Comments](c_comments_app.md#c_comments_app)
>## Hot Threads {#c_hot_threads}Displays the 25 most popular threads within the Collection, ordered by popularity.<!-- c_hot_threads.dita --> The Hot Threads view displays the 25 most popular threads within the Collection, ordered by popularity. This includes all content in the Collection, including manual posts, content from SocialSync and content from Curate.

>[!NOTE]
>
>Hot Threads is available on Comments, but not Live Blog or Chat.

For more information on enabling the Hot Threads view, please see Studio &gt; Network Settings.

## Previews {#section_xhh_2dl_wy}

Clicking ** `Hot Threads` ** at the top of the stream replaces the contents of the Collection with previews of up to 25 threads with the highest “popularity scores” from the Collection. A popularity score is calculated for each thread using Livefyre’s proprietary and evolving algorithm. The preview displays a top level comment, and up to 5 of the most popular replies, as well as the direct parent of each of these top 5 replies.
If there are no threads in the stream with a popularity score, no comments will be displayed, and users will see the message ** `There are not enough threads yet` ** and a link to ** `See what’s new` **.
The Hot Threads list is not real-time, and will update only when the page is refreshed or another view ( ** `Newest` ** or ** `Oldest` **) is selected. (If a comment is moderated and Bozo’d or trashed, it will be removed from the list immediately.)

## Breakout View {#section_zmf_ddl_wy}

From the preview, click ** `Show entire Thread` ** to replace the Hot Threads view with a breakout view of the thread in context, including every reply within that thread. (No other threads are displayed in the breakout view.) Click ** `Hot Threads` ** to return to the Hot Threads view.
Moderators can view all pending content in the breakout view and inline moderation is available. Likes, replies, edits and moderation actions will continue to stream in real-time in the breakout view.

## Posting from the Hot Threads View {#section_bmv_bdl_wy}

Posting a comment from the top comment box in the Hot Threads view will switch users back to the Newest view.
Replies or Likes posted in the Hot Threads view will appear in the stream without changing views. Sorting options and the comment notifier are not available in the Hot Threads view.
To optimize for performance, Livefyre caches data for up to 2 minutes. There may be a slight lag in the most recent Hot Threads that appear.

<a id="section_blk_ccj_h1b"></a>

Apps that use this feature:

* [Comments](c_comments_app.md#c_comments_app)
