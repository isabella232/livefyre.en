---
description: Importing ratings and reviews data to Livefyre.
seo-description: Importing ratings and reviews data to Livefyre.
seo-title: Importing Ratings and Reviews
solution: Experience Manager
title: Importing Ratings and Reviews
---

# Importing Ratings and Reviews


>## Import User Profiles, Content, Ratings, and Reviews {#c_importing_existing_data}
>Import your users and comments from an old system into Livefyre.

On this page:

* [](#c_importing_existing_data/section_gsm_ml1_c1b)
* [](#c_importing_existing_data/section_q1h_ll1_c1b)
* [](#c_importing_existing_data/section_krb_rk1_c1b)
* [](#c_importing_existing_data/section_hnr_nk1_c1b)
* [](#c_importing_existing_data/section_it3_mk1_c1b)
* [](#c_importing_existing_data/section_nf1_tj1_c1b)
* [](#c_importing_user_profiles)
    * [](#c_importing_user_profiles/section_hbh_4h1_c1b)
    * [](#c_importing_user_profiles/section_j3d_3h1_c1b)
    * [](#c_importing_user_profiles/section_stb_2n5_b1b)
  
* [](#c_importing_content)
    * [](#c_importing_content/section_vhm_vtt_b1b)
    * [](#c_importing_content/section_p4c_qtt_b1b)
    * [](#c_importing_content/section_ufj_jkn_b1b)
  
* [](#c_importing_ratings_and_reviews)
    * [](#c_importing_ratings_and_reviews/section_o1d_52n_b1b)
    * [](#c_importing_ratings_and_reviews/section_nxl_vcn_b1b)
    * [](#c_importing_ratings_and_reviews/section_vnz_3cn_b1b)
  
<!-- c_importing_existing_data.dita -->
Livefyre enables customers to import legacy comment and user profile data, allowing you to maintain user history in your new Livefyre App.

You will be asked to provide Livefyre with one file per site per import type (legacy and recent). For example, if you have three sites with both legacy and recent content, you will be asked to provide six files. After launch, we require one delta file per site, to bridge the gap between legacy and current content.

Please name and structure your files meaningfully. For example:

```
{network}_site-{siteid}_{date in mm-dd-yyyy}_{recent | legacy | delta}.json 

```
## Import Types {#section_gsm_ml1_c1b}

When importing, content must be split into two types:

**Recent Comments (or Interactive Comments): **include the most recent content posted prior to your launch date. (The exact time period for “Recent Comments” will be specified in your Livefyre contract.) Imported comments will look and behave as if posted after integration. Recent content is active and interactive.

**Legacy Comments (or Archived Comments): **include content posted previous to the specified cut-off point for your Recent Comments import. These comments will display in the stream, and may be styled to indicate that they are “archived” comments, but they will not be available in Studio, and will not support user interaction. Legacy content is archival, and not interactive.

>[!NOTE]
>
>Livefyre Comments and Chat imports are similarly structured. This document will refer to Comments or Content, but the process described applies to Chat as well.
Use the archiveHeaderTitle key to customize the text displayed for the `uicontrol  From the Archive` header.

## Import Process and Schedule {#section_q1h_ll1_c1b}

Work with your Strategic Account Manager to schedule and orchestrate the import process. Before your import begins, Livefyre will share a Box.com account with you, to which your data files (as .zip files) should be uploaded.

The import process spans three milestones:

* Sample Import Hand Off
* Production Import Hand Off
* Delta Import Hand Off
## Stage I: Sample Import Hand Off {#section_krb_rk1_c1b}

1. Export your data from your previous provider.
1. Prepare a sample for each site of Comment and User Profile data using the Format/Validation Standards described below (2MB or up to 500 records).
1. Test the sample files using Livefyre’s validator tool. This can be provided by your TIM or Support representative. This tool validates Comments (and Chat) files only. User files will be validated by Livefyre.
1. Correct any errors raised by the validator, and re-test your sample.
1. Once the validator passes your files without errors, provide the sample export of Comments and associated User Data to Livefyre by uploading the files to the Box.com account shared by your SAM.
   1.
   Livefyre will then perform an import of the sample data in the UAT/integration environment.
   
   **Please allow 3 days from Handoff date for the import process to complete.**
   
   
1. Upon completion of the sample import, QA the imported data in your integration environment.
1. Work with Livefyre to resolve any issues found during the sample data import.
## Stage ll: Production Import Hand Off (performed before launch) {#section_hnr_nk1_c1b}

1. Prepare a full export of Comment and User Data for all data previous to your launch date minus 5 days.
1. Provide Livefyre with these final data files 3-5 days before your launch date.
   1.
   Livefyre will then perform an import of the final data in the Production environment.
   
   Allow 3-5 days from Handoff date for the import process to complete.
   
   
## Stage lll: Delta Import Hand Off (if required) {#section_it3_mk1_c1b}

If there is data generated during the Production import, and before your launch date, a Delta import is required.

   1.
   Provide a delta export of data for the 5 days between initial import and launch date.
   
   >[!NOTE]
   >
   >Include all comments for a given Collection (not just the new comments since the production import) to guarantee a complete data set. Duplicates will be skipped by our importer.
   
1. Livefyre performs an import of the Delta in the Production environment. Allow 3 days from Handoff date for the import process to complete.
## Import Deltas {#section_nf1_tj1_c1b}

Depending on the size of the import, and the duration of the data load, it may become necessary to provide an import delta. If importing Recent Comments, it is only necessary to provide data created after the initial import, and during the data load. If importing Legacy Comments, full conversations must be provided.

When providing the delta import, include all comments for a given Collection (not just the new comments since the production import). This will guarantee a complete data set. Duplicates will be skipped by our importer.

When supplying a delta, any comments that refer to a parent comment with parent_id must include the parent comment in the data file as well.


>## Importing User Profiles {#c_importing_user_profiles}
>Import your existing user profiles to Livefyre.

<!-- c_importing_user_profiles.dita -->
To associate users with their existing content in Livefyre, you must import user data from your user management system before importing any legacy content. Only user accounts with associated content need be imported. Any user accounts not imported before launch will be automatically imported from your User Profile system into the Livefyre system upon first login.

Importing user profile data follows the standards described for importing Comments, with a few exceptions. For more information on Import Format and the Import Process, see Importing Content.

## User Data Formatting {#section_hbh_4h1_c1b}

To begin the import process, you must prepare your import data. Livefyre’s import system expects a specific file format of line-delimited JSON Blobs, with each file representing a site on your network, and each line within the file representing an individual Collection on that site.

Similar to Content import, User Profile files adhere to these rules:

* Profile Blobs must appear on a single line and may not include any literal endlines other than a single one at the end of each Blob.
* The top level id field must be unique to the user.
* The file must be UTF-8 formatted, all URLs must be fully qualified, user timestamps must be ISO-8601 compliant.
>[!NOTE]
>
>The files themselves are not valid JSON, but each line must be in JSON format.
The User Profile [ JSON schema ](https://json-schema.org/) is described in this Livefyre [ GitHub gist ](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/user_schema.json). Validators can be found in the language of your choice from the json-schema.org &gt; [ Implementations ](https://json-schema.org/implementations.html) page.

If you choose to import users from your existing user profile system, required fields include:

* **id: **your system’s user ID. It must match [a-zA-Z0-9-_])
* **display_name**:user’s display name or pseudonym which will be displayed on your public-facing site.
* **email**: required for Livefyre’s email notifications, this address is not visible on your public-facing site.
Use Livefyre’s Ping for Pull to update user fields after import. Ping Livefyre when one of your users updates their profile, then Livefyre will Pull down the requested user’s updated profile.

>[!NOTE]
>
>Provide user avatars only through Ping for Pull. You cannot import user avatars.
## Available User Parameters {#section_j3d_3h1_c1b}

The following parameters are used in the User Profile import process.

**Required fields**

**Optional fields**

## Example User Profile Format {#section_stb_2n5_b1b}

>[!NOTE]
>
>The following example lists both required and optional user profile import data.
```
{ 
 "id": "_u1", 
 "display_name": "John Smith", 
 "name": { 
 "formatted": "John Michael Smith", 
 "first": "John", 
 "middle": "Michael", 
 "last": "Smith" 
 }, 
 "email": "mohnsmith@gmail.com", 
 "tags": ["subscriber", "power_user"], 
 "profile_url": "https://site.com/johnsmith", 
 "settings_url": "https://site.com/settings", 
 "websites": ["https://johnsmith.com/blog/"], 
 "location": "Washington D.C., USA", 
 "bio": "Bob Dole talks in the third person", 
 "email_notifications": { 
 "comments": "never", 
 "moderator_comments": "immediately", 
 "moderator_flags": "immediately", 
 "replies": "immediately", 
 "likes": "often" 
 }, 
 "autofollow_conversations": true 
}
```

>## Importing Content {#c_importing_content}
>Importing user and comment data into Livefyre.

<!-- c_importing_content.dita -->
Import legacy content after your user profile data import is complete to allow Livefyre to link content to its author appropriately.

## Content Data Formatting {#section_vhm_vtt_b1b}

To begin the import process, you must prepare your import data. Livefyre’s import system expects a specific file format of line-delimited JSON Blobs, with each file representing a site on your network, and each line within the file representing an individual Collection on that site.

The Content [ JSON schema ](https://json-schema.org/) is described in this Livefyre [ GitHub gist ](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/conv_schema.json). Validators can be found in the language of your choice from the json-schema.org &gt; [ Implementations ](https://json-schema.org/implementations.html) page.

**File Format Standards**

A successful import must adhere to the following standards:

* Individual files may not contain multiple sites. Please create one file per site.
* Each line must be valid JSON, but the files do not need to be valid JSON. Do not include commas after each line.
* All Comments in a given Collection must appear in full on a single line. Do not include any literal endlines other than a single one at the end of each (Collection) Blob.
* Files must be UTF-8 formatted.
* Timestamps must be [ ISO-8601 compliant ](https://en.wikipedia.org/wiki/ISO_8601).
* URLs must be fully qualified. They must include https:// or https:// and domains must include the trailing /. For example:
    * https://web.livefyre.com/ or https://web.livefyre.com/index.html
  
* The top level id field must be unique to the content. (This id is often the CMS’s unique ID, but may also be the content’s URL, post number, or other identifying string. If using the content URL as the unique identifier, it is a best practice to MD5 or otherwise hash the identifier to meet field length restrictions.)
* To streamline the import process, do not import Collections that do not yet include comments. After implementation, Livefyre will automatically create a Collection with 0 comments the first time your App is loaded on the page.
* If not importing User Profiles, omit the author_id field from the Blob (unless you are preparing files for Livefyre’s archive import).
**HTML Standards**

* **Allowed HTML tags and attributes in comment bodies:**
    * Tags: a, span, label, p, br, strong, em, u, blockquote, ul, li, ol, pre, body, b, i
    * Attributes: href, target
  **Line breaks:** Line breaks in comments must be represented as &lt;p&gt;&lt;/p&gt; and &lt;br&gt; tags. n will not be accepted. Wrapping the entire comment in surrounding &lt;p&gt;&lt;/p&gt; tags is not required.
  
  
* **Do not use HTML entities in Collection Titles:** HTML entities like &lt;b&gt;, &lt;i&gt;, &lt;strong&gt;, and &lt;em&gt; must be removed from the Collection title. If included, they will be represented literally in the displayed Collection title in Studio.
* **Do not encode angle brackets in HTML tags: **The left and right angle bracket characters ( &lt; &gt; ) of HTML tags in body_html should not be encoded. If encoded, these tags will have no meaning and will be displayed literally in Studio.
  *
  **Escape quotations in tags: **Quotation marks in HTML tags must be backslash escaped.
  
  For example: &lt;a href=”https://www.baseart.fr/doc/sacguccifrance.php”&gt;gucci jeans&lt;a&gt;
  
  
* **Do not add extra attributes from anchor tags: **Additional attributes like rel=”nofollow” and rel=”bookmark” are not permitted. The additional invalid attributes will be stripped out during the import, and the anchor tag will be imported without them.
**Threaded Content**

To maintain threading in your imported content, adhere to the following rules:

  *
  **Comment ordering: **To preserve comment threading, parent content must be imported before child/reply content. Specifically, the top level ID of a comment must exist before a child comment references it as parent. An easy way to accomplish this is to list comments from oldest to newest date of creation.
  
  **Note: **Livefyre doesn’t keep a record of parent IDs after running a sample import. Parent IDs must be included in the delta file.
  
  
* **Threading with moderated comments: **To maintain threading in your reply structures, set the parent_id for every reply comment.
* **Deleted or Moderated comments: **There are two options for comments that have been deleted or moderated and have child replies:
      *
      **Import all comments: **Import all comments and replace the text of deleted or moderated comments with a standardized message.
      
      For example, if your original content structure follows this format:
      
      - A
      
      — B (deleted/moderated)
      
      — C
      
      —- DStructure the import file to replace the deleted content with a message:
      
      - A
      
      — B (replace body_html text. For example: “This comment has been deleted or moderated.”)
      
      — C
      
      —- D
      
      
      *
      **Import approved comments only: **Include only approved (non-moderated) comments and comments from users that have not been banned in the import. To preserve threading, replies to removed comments must specify the parent of the removed comment’s ID as the parent_id.
      
      For example, if content follows this format:
      
      - A
      
      — B (deleted/moderated)
      
      — C
      
      —- D Structure your import file to set the top level comment as the parent to the removed content’s child:
      
      - A
      
      — C (set parent_id to ID of A)
      
      — D
      
      
  
**Special Characters**

* **Encode non-ASCII special characters: **All non-ASCII special characters must be encoded, preferably with Python style encoding. For example, replace smartquotes (also known as typographer’s quotes ’ ) with u2019. (Do not escape the backslash; Livefyre requires the single backslash.)
## Available Content Parameters {#section_p4c_qtt_b1b}

The following parameters are used in the Content import process.

**Required**

**Optional fields**

## Example Comment Format {#section_ufj_jkn_b1b}

>[!NOTE]
>
>`codeph  parent_id` and `codeph  id` must be strings in your import file.
```
{ 
 "source": "https://www.somepartner.com/homepage/check-out-this-sneezing-panda.html", 
 "title": "Check out this sneezing panda!", 
 "created": "2010-07-05T23:07:15Z", 
 "id": "3042469", 
 
 "comments": [ 
 { 
 "id": "99770519", 
 "imported_display_name": "chris", 
 "author_id": "99999", 
 "body_html": "&lt;p&gt;OMG I love how cute the video is!&lt;/p&gt;", 
 "created": "2010-07-05T23:01:15Z" 
 }, 
 { 
 "id": "99770520", 
 "body_html": "&lt;p&gt;OMG I love how cute the video is!&lt;/p&gt;", 
 "created": "2010-07-05T23:01:15Z", 
 "author_id": "999999", 
 "imported_display_name": "chris", 
 "imported_email": "chris@livefyre.com", 
 "imported_url": "https://livefyre.com", 
 "parent_id": "99770519", 
 "likes": ["999998", "999990"] 
 } 
 ], 
 
 "tags": ["blog_post","news","sports"], 
 "allow_comments": true 
}
```

>## Importing Ratings and Reviews {#c_importing_ratings_and_reviews}
>Importing ratings and reviews data to Livefyre.

<!-- c_importing_ratings_and_reviews.dita -->
Importing your legacy ratings and reviews data allows you to maintain historic data in your Livefyre Ratings and Reviews Apps.

## Ratings and Reviews Data Formatting {#section_o1d_52n_b1b}

For Rating and Reviews specific imports, exclude endlines from the JSON record, and make sure that each Rating or Review appears on a single line.

The Reviews [ JSON schema ](https://json-schema.org/) is described in this Livefyre [ GitHub gist ](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/reviews_schema.json). Validators can be found in the language of your choice from the json-schema.org &gt; [ Implementations ](https://json-schema.org/implementations.html) page.

To import only Ratings and Reviews, and not the associated user profiles, follow the example JSON format below, and specify fields that begin with imported_. In this case, only imported_display_name is required. When using these fields, omit the author_id.

## Available Ratings and Reviews Parameters {#section_nxl_vcn_b1b}

The following parameters are used in the Ratings and Reviews import process.

**Required fields**

**Optional fields**

## Example Ratings and Reviews Format {#section_vnz_3cn_b1b}

>[!NOTE]
>
>The following sample data is for a Reviews Collection with multiple rating dimensions. If your Collection has only one dimension (such as overall/default), the dimensions field must be [‘default’], and the ratings fields in the reviews should only have one score.
Single-dimension review with required fields

```
{ 
 "source": "https://www.somepartner.com/homepage/check-out-this-sneezing-panda.html", 
 "title": "Check out this sneezing panda!", 
 "created": "2010-07-05T23:07:15", 
 "id": "3042469", 
 "dimensions": ['firmness', 'comfort', 'style'], 
 
 "reviews": [ 
 { 
 "id": "99770519", 
 "imported_display_name": "chris", 
 "title": "User's review title", 
 "body_html": "&lt;p&gt;OMG I love this product!&lt;/p&gt;", 
 "created": "2010-07-05T23:01:15", 
 "ratings": [70] 
 }, 
 ], 
}
```
Multi-dimension review with required fields

```
{ 
 "id": "99770519", 
 "imported_display_name": "chris", 
 "title": "User's review title", 
 "body_html": "&lt;p&gt;OMG I love this product!&lt;/p&gt;", 
 "created": "2010-07-05T23:01:15", 
 "ratings": [80, 100, 70] 
},
```
Multi-dimension review with additional fields

```
{ 
 "id": "99770520", 
 "imported_display_name": "chris", 
 "title": "User's review title", 
 "body_html": "&lt;p&gt;The product was just OK&lt;/p&gt;", 
 "created": "2010-07-05T23:01:15", 
 "ratings": [20, 30, 40] 
 "author_id": "999999", 
 "imported_email": "chris@livefyre.com", 
 "imported_url": "https://livefyre.com" 
},
```
Reviews with multiple subparts

```
{ 
 "id": "99770519", 
 "imported_display_name": "chris", 
 "title": "User's review title", 
 "body_html": "&lt;p&gt;OMG I love this product!&lt;/p&gt;", 
 "subparts": {"Pros":"Amazing tech breakthrough","Cons":"Short battery life"}, 
 "created": "2010-07-05T23:01:15", 
 "ratings": [80, 100, 70] 
},
```
>[!NOTE]
>
>Review subparts are used to define one or more customizable fields that you want to include in your reviews in addition to title and body.
