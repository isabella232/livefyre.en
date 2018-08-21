---
description: Listener count is a counter that tracks the number of site visitors for an App on a page and displays this number.
seo-description: Listener count is a counter that tracks the number of site visitors for an App on a page and displays this number.
seo-title: Listener Count
solution: Experience Manager
title: Listener Count
uuid: 0547ac0b-d493-45af-be73-a807204031ae
index: y
internal: n
snippet: y
translate: y
---

# Listener Count

Listener Count is the number of site visitors that have a browser open to the page on which an App is instantiated. This allows you to know how many site visitors are on the page at any given time, so you can track them while they watch streaming or live content in real time.

Livefyre's Listener count works like this: 

1. The site containing your App pings a Livefyre server every 60 seconds.
1. The Livefyre server responds with the number of site visitors on the page that displays the App (defined as the number of site visitors with a browser open to that page).
1. The number of site visitors on the page with the App displays on the App.
Apps that use this feature:

* [ Chat ](c_chat_app/c_chat_app.md#c_chat_app)
* [ Comments ](c_comments_app.md#c_comments_app)
* [ Reviews ](c_reviews_app/c_reviews_app.md#c_reviews_app)
![](assets/ListenerCount.jpg) 
## Listener Avatars {#section_wcn_kxp_vz}

The listener count displays a maximum of 10 avatars, and displays avatars only for those people who have clicked **[!UICONTROL  Follow]** for the conversation.

>[!NOTE]
>
>Due to space constraints, the mobile interface displays only the number of listeners, and a small “people” icon.

The Livefyre Listener Count displays the number of people actively on the page at any given time, plus the number of people following the conversation. If someone is on the page and following the conversation, that user will not be double counted. For example, if a user is on a page and clicks **[!UICONTROL  Follow]**, the listener count will not increase; if that user then clicks **[!UICONTROL  Unfollow]**, the count will not decrease.

Apps that use this feature:

* [ Chat ](c_chat_app/c_chat_app.md#c_chat_app)
* [ Comments ](c_comments_app.md#c_comments_app)
* [ Reviews ](c_reviews_app/c_reviews_app.md#c_reviews_app)
* [ Storify 2 ](c_storify2/c_storify2.md#c_storify2)
