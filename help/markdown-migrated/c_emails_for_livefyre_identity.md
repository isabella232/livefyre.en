---
description: 
seo-description: 
seo-title: Identity: Emails for Livefyre Identity
solution: Experience Manager
title: Identity: Emails for Livefyre Identity
---

# Identity: Emails for Livefyre Identity

<a id="section_j4h_5hs_p1b"></a>

Livefyre Identity sends the following emails:

* [](#c_emails_for_livefyre_identity/section_nd1_whs_p1b)
* [](#c_emails_for_livefyre_identity/section_ak5_xhs_p1b)
    * [](#c_emails_for_livefyre_identity/section_vyv_yhs_p1b)
  
* [](#c_emails_for_livefyre_identity/section_z2v_zhs_p1b)
    * [](#c_emails_for_livefyre_identity/section_kjp_c3s_p1b)
  
You can customize the look and feel of all Livefyre Identity emails in `uicontrol Integration Settings &gt; Email Notifications.`

## Password Reset Email {#section_nd1_whs_p1b}

Livefyre automatically sends a password reset email when a user tries to reset their password.

The password reset email looks like this:

**Subject:** Reset Password

**Body:**

Hey there *&lt;username&gt;*,

There was a request to change the password of your profile on *&lt;network name&gt;*.

If you requested this, please click the following link to choose a new password: *&lt;password reset URL&gt;*.

*&lt;Username&gt;*, *&lt;network name&gt;*, and *&lt;password reset URL&gt;* are all dynamically generated based on the site visitor and your network.

## Verification Email {#section_ak5_xhs_p1b}

You can send an email verifying the email address of a user. To send verification emails, you must turn on the option in **Integration Settings**&gt; **Livefyre Identity**.

The verification email looks like this:

**Subject:** Email Verification

**Body:**

Hello *&lt;username&gt;*,

Please click on the following link (or paste in your browser) to verify your account: *&lt;verification URL&gt;*.

This link will expire in 24 hours.

Thanks,

The *&lt;customer name&gt;* Team

*&lt;Username&gt;*, *&lt;network name&gt;*, and *&lt;verification URL&gt;* are all dynamically generated based on the site visitor and your network.

## Send an Email Verification to Users {#section_vyv_yhs_p1b}

You can send an email to a user to verify the email address they use to sign up for an account. To send a verification email:

1. In Studio, click on the gear icon to modify network settings.
1. Click **Integration Settings**&gt; **Livefyre Identity.**
1. Navigate to **Login Types**.
1. Click **Require Email Verification** to send an email to users that verifies the email address they use to sign up for an account.
1. Navigate to **Network Email** to configure the **Logo for Email**, the email address to use as the from address (**Email From**), and the display name to use for the from email address (**Email Display Name**).
## Welcome Email {#section_z2v_zhs_p1b}

You can send a welcome email to users. To send welcome emails, you must turn on the option in **Integration Settings** &gt; **Livefyre Identity**.

The welcome email looks like this:

**Subject:** Welcome to *&lt;customer name&gt;*

**Body:**

Hello *&lt;username&gt;*,

An account was created for you on *&lt;customer name&gt;*.

This account was created on *&lt;referral URL&gt;* from IP address *&lt;IP Address&gt;*.

If you did this, you can safely disregard this email.

If you didn’t do this, please contact support@livefyre.com.

Thanks

The *&lt;customer name&gt;* Team

*&lt;Username&gt;, &lt;customer name&gt;, &lt;referral URL&gt;,* and &lt;*IP Address&gt;* are all dynamically generated based on the site visitor and your network.

## Send a Welcome Email to a User {#section_kjp_c3s_p1b}

You can send a welcome email to a user after they sign up for an account. Studio sends this email after it sends a verification email, if you set up a verification email. To send a welcome email:

1. In Studio, click on the gear icon to modify network settings.
1. Click **Integration Settings &gt;****Livefyre****Identity****.**
1. Navigate to **Email Setting****s**.
1. Click **Send Welcome Emails To New Users** to enable sending emails.
1. Navigate to **Network****Email** to configure the **L****ogo****for Email**, the email address to use as the from address (**Email From**), and the display name to use for the from email address (**Email Display Name**).
