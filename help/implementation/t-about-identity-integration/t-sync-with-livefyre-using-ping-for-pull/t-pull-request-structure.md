---
description: Build the pull request structure to receive and respond to requests for access to your user identity system.
seo-description: Build the pull request structure to receive and respond to requests for access to your user identity system.
seo-title: Pull Request Structure
solution: Experience Manager
title: Pull Request Structure
uuid: bf6b9e45-d08a-48e6-acc6-e4fa56428d25

---

# Pull Request Structure{#pull-request-structure}

Build the pull request structure to receive and respond to requests for access to your user identity system.

Livefyre issues a Pull request to your endpoint URL.

For example, if your Pull endpoint URL is:

```
https://example.yoursite.com/some_path/?id={id}
```

the Livefyre Pull request to this endpoint will be:

```
https://example.yoursite.com/some_path/?id={id}&lftoken={UserAuthToken}
```

where `lftoken` is a JSON Web Token signed with your network key, and **[!UICONTROL {userAuthToken}]** is the user auth token generated by Livefyre.

1. Use `lftoken` to validate that requests to your Ping for Pull URL were sent by Livefyre and not a malicious agent.
1. For all incoming requests:

    * Ensure that the `lftoken` query string is present on the request.
    * Use the `validateLivefyreToken` method in the Livefyre libraries to ensure that `lftoken` was signed with your Network Key.
    
    * If `lftoken` is not present, or fails validation, do not allow your endpoint to respond with profile information. Instead, respond with a 403 (Forbidden) status code and no response body.

1. `userAuthToken` is generated by the Livefyre `buildUserAuthToken` method for the user, with user id “system”. This user is the first user created for every new network.
