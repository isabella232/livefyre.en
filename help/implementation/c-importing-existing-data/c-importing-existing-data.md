---
description: Import your users and comments from an old system into Livefyre.
seo-description: Import your users and comments from an old system into Livefyre.
seo-title: Importing Existing Data
solution: Experience Manager
title: Importing Existing Data
uuid: 2ac4ad48-d30e-455b-859e-879123db1a3e
index: y
internal: n
snippet: y
---

# Importing Existing Data{#importing-existing-data}

Import your users and comments from an old system into Livefyre.

Livefyre enables customers to import legacy comment and user profile data, allowing you to maintain user history in your new Livefyre App.

You will be asked to provide Livefyre with one file per site per import type (legacy and recent). For example, if you have three sites with both legacy and recent content, you will be asked to provide six files. After launch, we require one delta file per site, to bridge the gap between legacy and current content.

Please name and structure your files meaningfully. For example:

```
{network}_site-{siteid}_{date in mm-dd-yyyy}_{recent | legacy | delta}.json

```

## Import Types {#section_gsm_ml1_c1b}

When importing, content must be split into two types:

**Recent Comments (or Interactive Comments):** include the most recent content posted prior to your launch date. (The exact time period for “Recent Comments” will be specified in your Livefyre contract.) Imported comments will look and behave as if posted after integration. Recent content is active and interactive.

**Legacy Comments (or Archived Comments):** include content posted previous to the specified cut-off point for your Recent Comments import. These comments will display in the stream, and may be styled to indicate that they are “archived” comments, but they will not be available in Studio, and will not support user interaction. Legacy content is archival, and not interactive.

>[!NOTE]
>
>Livefyre Comments and Chat imports are similarly structured. This document will refer to Comments or Content, but the process described applies to Chat as well.

Use the archiveHeaderTitle key to customize the text displayed for the **[!UICONTROL From the Archive]** header.

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
1. Livefyre will then perform an import of the sample data in the UAT/integration environment.

   **Please allow 3 days from Handoff date for the import process to complete.**

1. Upon completion of the sample import, QA the imported data in your integration environment.
1. Work with Livefyre to resolve any issues found during the sample data import.

## Stage ll: Production Import Hand Off (performed before launch) {#section_hnr_nk1_c1b}

1. Prepare a full export of Comment and User Data for all data previous to your launch date minus 5 days.
1. Provide Livefyre with these final data files 3-5 days before your launch date.
1. Livefyre will then perform an import of the final data in the Production environment.

   Allow 3-5 days from Handoff date for the import process to complete.

## Stage lll: Delta Import Hand Off (if required) {#section_it3_mk1_c1b}

If there is data generated during the Production import, and before your launch date, a Delta import is required.

1. Provide a delta export of data for the 5 days between initial import and launch date.

   >[!NOTE]
   >
   >Include all comments for a given Collection (not just the new comments since the production import) to guarantee a complete data set. Duplicates will be skipped by our importer.

1. Livefyre performs an import of the Delta in the Production environment. Allow 3 days from Handoff date for the import process to complete.

## Import Deltas {#section_nf1_tj1_c1b}

Depending on the size of the import, and the duration of the data load, it may become necessary to provide an import delta. If importing Recent Comments, it is only necessary to provide data created after the initial import, and during the data load. If importing Legacy Comments, full conversations must be provided.

When providing the delta import, include all comments for a given Collection (not just the new comments since the production import). This will guarantee a complete data set. Duplicates will be skipped by our importer.

When supplying a delta, any comments that refer to a parent comment with parent_id must include the parent comment in the data file as well.
