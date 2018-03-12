---

title: Syntax sample page
description: The role of the Experience Cloud ID service in the Adobe Experience Cloud.
author: gipaul
doc type: article
SEO title:
SEO description:
archetype: administrator
machine translation: n

inherited from yaml 
business unit: digital-experience
cloud: experience-cloud
solution: core-services-id-service
guide topic: overview
guide subtopic: getting-started

---
# Sample showing syntax
The role of the Experience Cloud ID service in the Adobe Experience Cloud.

# The Experience Cloud ID Service: A Foundational Element of Core Services
The Experience Cloud ID service enables the common identification framework for the Experience Cloud Core Services, solutions, and customer attributes and audiences in the People core service. It works by assigning a unique, persistent ID to a site visitor. 

When your organization implements the ID service, this ID lets you identify the same site visitor and their data in different Experience Cloud solutions

![](media/getting-started-testpage/with-without-id-service.png "Identifying a site visitor with the Experience Cloud ID Service")

The ID service can also replace the different solution-specific IDs (e.g., Analytics AID). And, through the Customer IDs and Authentication States functionality, the ID service lets you pass in your own customer IDs to the Experience Cloud. 

[!Important]
Keep in mind, however, that the ID service only works with the solutions you're already subscribed to. It won't provide access to other products if you're not signed up for them. 

Going forward, the ID service is an integral component of many current and future Experience Cloud features, enhancements, and services. Currently, the ID service supports Analytics, Audience Manager, and Target. And, it is required if you want to participate in the Adobe Experience Cloud Device Co-op. 

If you have not implemented the ID service, now is the time to start considering a migration strategy. For more information about the importance and role of the ID service, see [Why the Experience Cloud ID Service Should be on Your Radar](../getting-started/test-page-for-links.md).

# Feature Summary
To sum up, the ID service:

- Creates a common key or ID which can be used to link profiles and identities.
- Uniquely identifies a device across multiple solutions.
- Sets a first-party cookie in customer’s domain to ensure tracking on same domain. See Experience Cloud.
- Receives aliases and ID mappings from Experience Cloud customers and partners.
- Manages ID synchronization within the Experience Cloud.
- Supports ID synchronization with different third-parties across the ad tech ecosystem.

# ID Service Requirements
Your solution and other Adobe code libraries [must meet these requirements](../getting-started/test-page-for-links.md) before you can use the ID service.



---


:::ReadNext What to read next
[How it works - Cookies and the Experience Cloud ID Service](../getting-started/getting-started-cookies-id-service.md)

