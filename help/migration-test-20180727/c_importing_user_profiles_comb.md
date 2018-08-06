---
description: Import your existing user profiles to Livefyre.
seo-description: Import your existing user profiles to Livefyre.
seo-title: Importing User Profiles
title: Importing User Profiles
uuid: 00167390-ff3f-4abc-85c7-c69e6511622b
index: y
internal: n
snippet: y
translate: y
---

# Importing User Profiles

## Importing User Profiles {#c_importing_user_profiles}Import your existing user profiles to Livefyre.<!-- c_importing_user_profiles.dita --> To associate users with their existing content in Livefyre, you must import user data from your user management system before importing any legacy content. Only user accounts with associated content need be imported. Any user accounts not imported before launch will be automatically imported from your User Profile system into the Livefyre system upon first login.
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

The User Profile [JSON schema](https://json-schema.org/) is described in this Livefyre [GitHub gist](https://github.com/Livefyre/import-tools/blob/master/lfvalidator/jsonschema/user_schema.json). Validators can be found in the language of your choice from the json-schema.org &gt; [Implementations](https://json-schema.org/implementations.html) page.
If you choose to import users from your existing user profile system, required fields include:

* **id:**your system’s user ID. It must match [a-zA-Z0-9-_])
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
