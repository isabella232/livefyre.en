# Table of Contents

+ Announcements
+ Access Training Videos
+ Product: Apps
    + Create an App
    + Carousel
        + Carousel Features
        + Create a Carousel Using Studio
        + Customize a Carousel Using Studio
        + Localize a Carousel
    + Chat
        + Chat Customizations
        + Chat Features
    + Comments
        + Comments Features
        + Comments Customizations
    + Feature Card
        + Feature Card Customizations
    + Filmstrip
        + Filmstrip Features
        + Filmstrip Customizations
    + Live Blog
        + Live Blog Features
        + Live Blog Customizations
    + Map
        + Map Features
        + Map Customizations
    + Media Wall
        + Media Wall Features
        + Media Wall Customizations
    + Mosaic
        + Mosaic Features
        + Mosaic Customizations
    + Polls
        + Add a Poll to a Comments or Live Blog App
        + Add Images to a Poll
        + Polls Customizations
    + Reviews
        + Creating a Reviews App
        + Post a Review
    + Sidenotes
        + Sidenotes Features
        + Sidenotes Customizations
        + Best Practicies for Sidenotes
    + Storify 2
        + Configuration Options
        + Storify Settings
        + Use Google AMP with Storify 2
        + Create a Story
        + Add Social Content
        + Add Text
        + Preview a Story
        + Publish a Story
        + Review History
        + Working with Multiple Editors on the Same Story
        + Use Streams to Add Social Content to your Story
        + Pin a Post to Storify 2
        + Navigation Guide
        + Add a Navigation Guide to a Storify 2
        + Add a Title to the Navigation Guide
        + Add Posts to the Navigation Guide
        + Set the Number of Posts in the Navigation Guide
        + Make the Navigation Guide Sticky
        + Move the Navigation Guide
    + Trending
        + Trending Features
        + Trending Customizations
    + Upload Button
        + Upload Button Customizations
        + Upload Button Text Strings
+ Product: App Features
    + Accessibility Features
    + Authentication Features
    + Content Behavior Features
    + Collection and Content Tags
    + Custom HTML
    + Engagement Features
    + Listener Accounts
    + Miscellaneous Features
    + Moderation and Filtering
        + Setting Up Moderation
        + Restrict Content from Twitter Users
        + Ban IP Addresses
        + Using the Profanity Filter
        + Moderate Users
        + Moderate Content Using ModQ
        + Add a Trashed Item Back into an App
        + ModQ Keyboard Shortcuts
        + Moderate Content from a Stream
        + Moderate Content using App Content
        + SAFE Rules            
    + Notifications Features
    + On+Site Contribution Features
    + Referral Tracking
    + Smart Tags
    + Social Sharing
    + SocialSync
    + Styling Features
    + Translation and Custom Text Strings
    + UGC Commerce
+ Product: Library
    + Assets
        + Create Asset Folders
        + Manage Asset Folders
        + View Asset Details
        + Publish Assets to Apps
        + Search Saved Assets in the Library
    + Search for Content from Twitter and Instagram Using the Social Search
    + Search for YouTube Content
    + Search for Twitter Content
    + Search for Instagram Content
    + View Content Details
    + Save Content to Asset Library
    + Associate Products with Content Using the Library
    + Publish Content
    + App Content Tab
+ Product: Streams
    + Create a New Stream
    + Add Rules for your Stream
    + Stream Rule Options for All Stream Rules
    + Facebook Rules
    + Facebook Page Rules
    + Email Rules
    + Instagram Rules
    + Instagram Content Guidelines
    + Tumblr Rules
    + Twitter Rules
    + Throttling and Frequency of Tweets
    + YouTube Rules
    + RSS Rules
+ Product: Requesting Rights
    + Managing Rights Requests
    + Set Up Rights Management
    + Send Rights Request from the Library
    + Send Rights Request from ModQ
    + Send Rights Request from App Content
    + View Rights Activity History
    + Manage Content with a Pending Rights Requests from the Asset Library
    + Manage Content with a Pending Rights Request from App Content
    + Manually Grant or Revoke Rights for an Asset from the Asset Library
    + Manually Grant or Revoke Rights for an Asset from the App Content
+ Product: Livefyre Mobile App
    + Log in to the Livefyre Mobile App
    + Create a Post Using the Livefyre Mobile App
    + Delete Media from a Post Using the Livefyre Mobile App
    + Save Post as a Draft Using the Livefyre Mobile App
    + Switch Networks Using the Livefyre Mobile App
    + Publish a Post to Storify 2 Using the Livefyre Mobile App
+ Users: Managing Studio and Livefyre Network Users
    + Search for Users
    + Viewing Account Details
    + Ban a User
    + Whitelist a User
    + Link User Accounts
    + Set up Network Email
    + Users Switching Networks
    + User Sync
+ Users: Creating User Accounts
    + Invite a User to Create a Studio Account
    + Accept an Invitation to Create a Studio Account
    + Log into Studio
    + Manage Studio Permissions for Users
    + User Roles and Permissions
+ Configure Social Accounts
    + Add a Social Account
    + About Instagram Accounts
    + Configure Social Account for Twitter
    + Refresh a Token for a Social Account
+ Settings: Other
    + Set Up Credentials
    + Add a Site to a Network
    + Translation Sets
        + Create and Modify Translation Sets
        + Apply a Translation Set to a Network
        + Apply a Translation Set to a Site
        + Delete a Translation Set
        + Localize Strings
        + Review Text Strings
        + Sidenotes Text Strings
    + SSL Enforcement
        + SSL Checklist
    + Privacy Requests (GDPR-Ready)
        + Privacy Request FAQs
        + Create  Privacy Request
        + View a Privacy Report
        + userPrivacyOptOut
        + userPrivacyMaskDelegate
        + userPrivacyVideoWhitelist
+ Developers: Getting Started with Livefyre Integration
    + Implementation Process
        + App Integration Types
        + Architecture
        + Embed an App
        + Add Authentication to an App using Livefyre.js
        + Build Server Side Tokens
        + CollectionMetaToken
        + User Auth Token
+ Developer Docs
    + Create a Collection Using the Collection Meta Token
    + Creating a Checksum
    + Identity: Identity Integration
        + Authentication Package
        + AuthDelegate Object
        + Posting User Permissions to External Systems (Optional)
        + Implementing SSO
            + Debugging Auth Delegate
        + Sync with Livefyre Using Ping for Pull
            * Build the Pull Endpoint
            * Register the Endpoint with Studio
            * Build the Ping
            * Pull Request Structure
            * Build the Ping for Pull Response    
    + Identity: Livefyre Identity
        + Identity: Your Identity Service
        + Enable Lifeyre Identity
        + Create Your Social Apps
        + Using Studio to Connect Your Social Apps to Your Livefyre Implementation
        + Add Livfyre.js to the Page
        + Initialize Livefyre Identity
        + Emails for Livefyre Identity
        + Identity: Janrain Capture/Backplane              
    + Importing Existing Data
        + Importing User Profiles
        + Importing Content
        + Importing Ratings and Reviews
    + Installation
        + Classes and Methods
        + Network Methods
        + setSSL Network Method
        + buildLivefyreToken Network Method
        + buildUserAuthToken Network Method
        + validateLivefyreToken Network Method
        + setUserSyncUrl Network Method
        + syncUser Network Method
        + getUrn Network Method
        + getUrnForUser Network Method
        + getNetworkName Network Method
        + getSite Network Method
        + Network Class Methods
        + Collection Class Methods
        + createOrUpdate Collection Method
        + buildCollectionMetaToken Collection Method
        + buildChecksum Collection Method
        + getCollectionContent Collection Method
        + getUrn Collection Method
        + Site Class Methods
        + buildBlogCollection Site Method
        + buildChatCollection Site Method
        + buildCommentsCollection Site Method
        + buildCountingCollection Site Method
        + buildRatingsCollection Site Method
        + buildReviewsCollection Site Method
        + buildSitenotesCollection Site Method
        + buildCollection Site Method
        + getUrn Site Method
        + Examples
    + Mobile SDKs
        + Livefyre iOS SDK
        + Android SDK
    + Livefyre.js
    + Creating Livefyre Tokens C#
    + Implement a Visualization App
    + App Integrations
    + App Customizations
        + Change Display Options
        + CSS Classes
        + Storify CSS Classes
        + Translation Sets
        + Date Time Stamp
        + Move the Livefyre Logo
        + Restrict Media
        + Hide App Elements
        + Change @mention Icon
        + Highlight Content
        + Feature Content
        + Enable Featuring Content in Studio
        + Select Content to Feature from an App
        + Select Content to Feature from Studio
        + Use CSS to Style Featured Content
        + Feature APIs
        + Connceting Janrain to Livefyre using AuthDelegate
        + Aggregated Featured Content Using the Featured APIs
        + Style User Group Content
        + Adding Users to Groups
        + Applying Custom Styles
        + Add Custom Buttons
        + JavaScript Events Definitions and Examples
        + Javascript Events for Visualization Apps
        + Javascript Events for Media Wall
        + Javascript Events for Conversation Apps
        + Embed a Comments App
        + Referral Tracking
        + Device and Browser Support
        + Twitter Display Requirements
    + Stress Test Policy
    + Analytics
        + Use Livefyre with Adobe Analytics And Dynamic Tag Manager (DTM)
        + Use Livefyre with Other Analytics Tool
        + Livefyre Analytics Events
    + Integrating Livefyre with AEM
    + Advanced Topics
        + Display Comment Count
        + Enabling Social Sharing
        + Activity Stream
        + Bootstrap HTML
        + Change Collection
        + Multiple Collections
        + Switch Core App Types
        + Social Counter
+ Livefyre Release Notes
    + Previous Release Notes
        + May 24, 2018
        + May 17, 2018
        + May 10, 2018
        + April 26, 2018
        + April 12, 2018
        + March 23, 2018
        + March 8, 2018
        + February 15, 2018
        + February 1, 2018
        + January 18, 2018
        + 2017 Release Notes (lets archive this.. or put all of them on one page)
