---
description: Grab the post and comment counts for certain collections to display on your index pages.
seo-description: Grab the post and comment counts for certain collections to display on your index pages.
seo-title: Display Comment Count
solution: Experience Manager
title: Display Comment Count
---

# Display Comment Count

Livefyre’s `codeph  CommentCount.js` allows you to fetch the content counts for collections on your site. Although Apps will show the comment count for the current collection, having these counts syndicated across your site can be useful. This feature is especially useful if you don’t persist content in your database (or if your CMS database is not synced with Livefyre).

>1. Load the JavaScript.
>   To use `codeph  CommentCount.js`, first embed the JavaScript file in the `codeph  &lt;head&gt;` section of the page or template where you’d like to use it.
>   
>   ```
>   &lt;script 
>    type="text/javascript" 
>    data-lf-domain="{network name (domain.fyre.co)}" 
>    src="//cdn.livefyre.com/libs/commentcount/v1.0/commentcount.js"&gt; 
>   &lt;/script&gt;
>   ```
>   
>   
>1. Bind the HTML Element.
>   Once the script is loaded, it will attempt to find other elements on the page with a class name of `codeph  livefyre-commentcount`. For each of these elements, the script will look for `codeph  data-lf-site-id` and `codeph  data-lf-article-id` HTML attributes, and will use these to fetch content from Livefyre and update each element with the latest value.
>   
>   For example, the following element would be updated:
>   
>   ```
>   &lt;span class="livefyre-commentcount" data-lf-site-id="{site_id}" data-lf-article-id="{article_id}"&gt; 
>   0 Comments 
>   &lt;/span&gt;
>   ```
>   >[!NOTE] {importance="high"}
>   >
>   >The`codeph  CommentCount.js` code checks for a numeric value to update with the actual count. Be certain to include a numeric value between the tags.
>   **Example 1** (Using the URL as the article ID):
>   
>   ```
>   &lt;span class="livefyre-commentcount" data-lf-site-id="311458" data-lf-article-id="http://mikesoldner.com/blog.php"&gt; 
>   0 Comments 
>   &lt;/span&gt;
>   ```
>   **Example 2** (Using a numbered system as the article ID):
>   
>   ```
>   &lt;span class="livefyre-commentcount" data-lf-site-id="311458" data-lf-article-id="25"&gt; 0 Comments &lt;/span&gt;
>   ```
>   
>   
>1. Configure Options.
>   For more control over how the content counts are replaced, call `codeph  LF.CommentCount()` and pass in an object containing the configuration options. Make sure to call the function after all of the elements that need to be replaced are in the DOM. The best place to call this method is in the footer, so it happens when the DOM is loaded, but prior to document and window ready events.
>   
>   We allow the following configuration options:
>   
>   **Example**:
>   
>   ```
>   >   &lt;script type="text/javascript"&gt; LF.CommentCount({ 
>    replacer: function(element, count) { 
>    element.innerHTML = count +' Comment'+ (count === 1 ? '' : 's'); 
>    } 
>    }); 
>   &lt;/script&gt;
>   ```
>   >[!NOTE]
>   >
>   >Use the replacer to customize or internationalize the comment count message.
>   
>   
>   
