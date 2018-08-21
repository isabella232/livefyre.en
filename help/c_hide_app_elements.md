---
description: Remove standard Livefyre App components from your App.
seo-description: Remove standard Livefyre App components from your App.
seo-title: Hide App Elements
solution: Experience Manager
title: Hide App Elements
uuid: 4cbc9189-b994-447c-967c-6c10a0c881f1
index: y
internal: n
snippet: y
translate: y
---

# Hide App Elements

Use CSS to hide default Livefyre App elements from your page, allowing you to customize the user experience to fit your needs.

To hide elements from the App, simply set display to none.

Examples:

```
/* Hide the 'reply' button */ 
.fyre-comment-reply { 
    display: none !important; 
} 
  
/* Hide all user avatars */ 
.fyre-comment-user .fyre-mention-item-avatar .fyre-listener-avatars .fyre-avatar fyre-user-avatar-25 { 
    display: none !important; 
} 
.fyre-comment-head .fyre-comment-body .fyre-comment-footer .fyre-comment-divider { 
    margin-left: 0; 
} 
  
/* Hide 'Edit Profile' link */ 
.fyre-edit-profile-link { 
    display: none !important; 
} 
  
/* Hide 'Logout' link */ 
.fyre-logout-link { 
    display: none; 
} 
  
/* Hide 'Comment Notifier' */ 
.fyre-notifier-message { 
    display:none; 
}
```
