---
description: Build the pull endpoint to receive and respond to requests for access to your user identity system.
seo-description: Build the pull endpoint to receive and respond to requests for access to your user identity system.
seo-title: Build the Pull Endpoint
solution: Experience Manager
title: Build the Pull Endpoint
uuid: ea5ad49d-c20e-4343-b47b-40893dcbf721
index: y
internal: n
snippet: y
translate: y
---

# Build the Pull Endpoint

Build the pull endpoint to receive and respond to requests for access to your user identity system.

1. Create an HTTPS endpoint that receives Livefyre requests and responds with a JSON object that contains the latest user data.

   >[!NOTE]
   >
   >This endpoint must be accessible. It is also strongly recommended that both requests and responses be sent over the HTTPS protocol.

1. Register the Endpoint with Studio.