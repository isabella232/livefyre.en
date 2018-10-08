---
description: Answers to Frequently Asked Questions (FAQs) about GDPR-Ready Privacy Requests.
seo-description: Answers to Frequently Asked Questions (FAQs) about GDPR-Ready Privacy Requests.
seo-title: Privacy Request FAQs
solution: Experience Manager
title: Privacy Request FAQs
uuid: 081b8cc8-6d1b-408c-805c-b5313441949b
index: y
internal: n
snippet: y
translate: y
---

# Privacy Request FAQs

Answers to Frequently Asked Questions (FAQs) about GDPR-Ready Privacy Requests.

* **How can site visitors opt out of being tracked on a site that uses Livefyre Apps?**When a site visitor opts out, the customer implementation must indicate to Livefyre that the user has opted out before instantiating an App. Livefyre has created a way to do this with the JavaScript option, `userPrivacyOptOut`. For more on how to use `userPrivacyOptOut`, see [](../c_gdpr_compliance/c_userprivacyoptout.md#c_userprivacyoptout).

  When the `userPrivacyOptOut` flag is set to true, any Apps on the page will not transmit data to Livefyre servers by using cookies or another method. Livefyre will then not update local storage with data that could be used to track site visitors. If a source doesn't support a proxy, then Livefyre displays a mask on the content unless a user clicks on the video and approves the potential tracking from that source.

  If you use Livefyre Identity, users can choose to delete their profile or create a report of data tracked for their user account.

* **How do I prevent collecting future content from a site visitor who has opted out?**Use `userPrivacyOptOut` with `livefyre.js` on a webpage that uses Livefyre Apps. For more on `userPrivacyOptOut`, see [](../c_gdpr_compliance/c_userprivacyoptout.md#c_userprivacyoptout).

* **How do I generate a report and delete the data for App Users or owners of social accounts?**[](../c_gdpr_compliance/c_privacy_requests.md#c_privacy_requests) to generate a report and delete user data from Apps.

* **How do I remove all content for a visitor?**Livefyre does not maintain persistent information about site visitors, except in the form of cookies to uniquely identify them for Livecount features. Livecount is a transient and real time count of visitors on the site. No history is retained after the visitor leaves or clears cookies.

  [](../c_gdpr_compliance/c_privacy_requests.md#c_privacy_requests) to delete the account. Livefyre deletes or makes the user profile and any associated records anonymous. 

* **How do I remove content for a registered user?**[](../c_gdpr_compliance/c_privacy_requests.md#c_privacy_requests) to delete the account. The user profile and any associated records will be completely destroyed. 

  >[!NOTE]
  >
  >This action cannot be undone.

* **How do I produce a report of data tracked of a current or former employee?**[](../c_gdpr_compliance/c_view_a_privacy_report.md#c_view_a_privacy_report) to generate a report of data tracked for a user account.

