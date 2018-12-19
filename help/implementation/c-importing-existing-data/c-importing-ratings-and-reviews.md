---
description: Importing ratings and reviews data to Livefyre.
seo-description: Importing ratings and reviews data to Livefyre.
seo-title: Importing Ratings and Reviews
solution: Experience Manager
title: Importing Ratings and Reviews
uuid: 5c3386e6-7622-41f3-ac25-92bc6ab846f7
index: y
internal: n
snippet: y
---

# Importing Ratings and Reviews{#importing-ratings-and-reviews}

Importing ratings and reviews data to Livefyre.

On this page:

* [](#c_importing_ratings_and_reviews/section_o1d_52n_b1b) 
* [](#c_importing_ratings_and_reviews/section_nxl_vcn_b1b) 
* [](#c_importing_ratings_and_reviews/section_vnz_3cn_b1b)

Importing your legacy ratings and reviews data allows you to maintain historic data in your Livefyre Ratings and Reviews Apps.

## Ratings and Reviews Data Formatting {#section_o1d_52n_b1b}

For Rating and Reviews specific imports, exclude endlines from the JSON record, and make sure that each Rating or Review appears on a single line.

The Reviews [JSON schema](https://json-schema.org/) is described in this Livefyre [GitHub gist](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/reviews_schema.json). Validators can be found in the language of your choice from the json-schema.org > [Implementations](https://json-schema.org/implementations.html) page.

To import only Ratings and Reviews, and not the associated user profiles, follow the example JSON format below, and specify fields that begin with imported_. In this case, only imported_display_name is required. When using these fields, omit the author_id.

## Available Ratings and Reviews Parameters {#section_nxl_vcn_b1b}

The following parameters are used in the Ratings and Reviews import process.

**Required fields**

* **source:** ***required* string **The site on which the Review originated.

* **title:** ***required* string **The title for the Collection to which the Review was posted.

* **created:** ***required* timestamp **The ISO-8601 compliant timestamp for the moment the Collection in which the Review was posted was created. For example: “2010-07-05T23:01:15Z”

* **id (source):** ***required* string **The article ID you chose to uniquely identify a Collection within your site, encoded using Base64. This parameter is limited to 150 characters.

* **dimensions:** ***required* array** An array of strings for each type of dimension that this Collection will use. If this is not specified, only 1 dimension will be allowed.For example, to allow users to rate your product on ‘design’, ‘features’, and ‘performance’, set the array to: dimensions: [‘design’, ‘features’, ‘performance’]

* **id (reviews):** ***required* string **Your system’s internal content identifier, used by the importer to relate children using their parent_id.

* **imported_display_name:** ***required* string **The display name of the user. This will be rendered with Livefyre content posted by the user.

* **title:** ***required* string **User’s review title.

* **body_html:** ***required* string **The text string for the Review. Only tags <p> and <a>, and only the href attribute, are allowed.

* **created:** ***required* timestamp **The ISO-8601 compliant timestamp for the Comment’s creation. For example: “2010-07-05T23:01:15Z”

* **ratings:** ***required* array **An array of integers (from 1-100) which represent the author’s rating for each of your defined dimensions. The number of items in the array must equal the number of defined dimensions.

**Optional fields**

* **author_id:** **(optional) string **The userId of the user in your profile system. This must be unique across all users in your Network, and must never change. Max length = 255 characters.

* **imported_email:** **(optional) string **Used for gravatars, and not displayed publicly.

* **imported_url:** **(optional) string **A user provided website.

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
         "body_html": "<p>OMG I love this product!</p>",
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
   "body_html": "<p>OMG I love this product!</p>",
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
   "body_html": "<p>The product was just OK</p>",
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
   "body_html": "<p>OMG I love this product!</p>",
   "subparts": {"Pros":"Amazing tech breakthrough","Cons":"Short battery life"},
   "created": "2010-07-05T23:01:15",
   "ratings": [80, 100, 70]
},
```

>[!NOTE]
>
>Review subparts are used to define one or more customizable fields that you want to include in your reviews in addition to title and body.

