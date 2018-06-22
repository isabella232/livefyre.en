---
description: Importing ratings and reviews data to Livefyre.
seo-description: Importing ratings and reviews data to Livefyre.
seo-title: Importing Ratings and Reviews
solution: Experience Manager
title: Importing Ratings and Reviews
---

# Importing Ratings and Reviews

On this page:

* [](#c_importing_ratings_and_reviews/section_o1d_52n_b1b)
* [](#c_importing_ratings_and_reviews/section_nxl_vcn_b1b)
* [](#c_importing_ratings_and_reviews/section_vnz_3cn_b1b)
Importing your legacy ratings and reviews data allows you to maintain historic data in your Livefyre Ratings and Reviews Apps.

## Ratings and Reviews Data Formatting {#section_o1d_52n_b1b}

For Rating and Reviews specific imports, exclude endlines from the JSON record, and make sure that each Rating or Review appears on a single line.

The Reviews [JSON schema](http://json-schema.org/) is described in this Livefyre [GitHub gist](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/reviews_schema.json). Validators can be found in the language of your choice from the json-schema.org &gt; [Implementations](http://json-schema.org/implementations.html) page.

To import only Ratings and Reviews, and not the associated user profiles, follow the example JSON format below, and specify fields that begin with imported_. In this case, only imported_display_name is required. When using these fields, omit the author_id.

## Available Ratings and Reviews Parameters {#section_nxl_vcn_b1b}

The following parameters are used in the Ratings and Reviews import process.

**Required fields**

**Optional fields**

## Example Ratings and Reviews Format {#section_vnz_3cn_b1b}

>[!NOTE]
>
>The following sample data is for a Reviews Collection with multiple rating dimensions. If your Collection has only one dimension (such as overall/default), the dimensions field must be [‘default’], and the ratings fields in the reviews should only have one score.
Single-dimension review with required fields:

```
{
 "source": "http://www.somepartner.com/homepage/check-out-this-sneezing-panda.html",
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
Multi-dimension review with required fields:

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
 "imported_url": "http://livefyre.com"
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
