---
description: The Livefyre.js Auth package ensures that all social components on your page can discover a single authentication integration.
seo-description: The Livefyre.js Auth package ensures that all social components on your page can discover a single authentication integration.
seo-title: Initialize Livefyre Identity
title: Initialize Livefyre Identity
uuid: 7e89b34e-da15-4a92-a759-cb300e05a154
index: y
internal: n
snippet: y
---

# Initialize Livefyre Identity{#initialize-livefyre-identity}

The Livefyre.js Auth package ensures that all social components on your page can discover a single authentication integration.

Livefyre provides an `lfep-auth-delegate` package that will make an appropriate auth delegate for you. Auth must be provided an AuthDelegate object that knows how to perform authentication actions, like login and logout.

1. Add Livefyre.js to your webpage.
1. To tell Auth to delegate these actions to Livefyre Identity, add the following:

   ```
   Livefyre.require([ 
     'livefyre-auth', 
     'identity' 
     ], function (auth, Identity) { 
       var identity = new Identity({ 
         app: "https://identity.livefyre.com/{networkName}.fyre.co" 
       }); 
    auth.delegate( identity ); 
    });
   ```

