---
description: You can create Stream rules that pull content from Twitter.
seo-description: You can create Stream rules that pull content from Twitter.
seo-title: Twitter Rules
solution: Experience Manager
title: Twitter Rules
uuid: ece2e9b3-b442-4bff-a490-34fbbef13026
index: y
internal: n
snippet: y
translate: y
---

# Twitter Rules

Create Twitter rules based on hashtags, keywords, @mentions, or author.
Adding ** ` Words` ** and a ** ` Username` ** for your rule will return content which includes both entries.

>[!NOTE]
>
>Livefyre adheres to Twitter display guidelines, and customers are responsible for adhering to these guidelines as well. For more information, please see Twitter’s documentation on their[ Display Requirements ](http://dev.twitter.com/terms/display-requirements). 

To create Twitter Rules to pull content from Twitter feeds into your App or Folder, you can filter by:

* ** ` Keywords` ** 
    * Enter ** ` Keywords` **to be included in, or excluded from your Twitter stream. Specifying values for both the ** ` Contains any of these words` ** and ** ` Does not contain any of these words` ** fields will return Tweets which contain the first, and do not contain the second. Multiple values for a single field may be entered, and will return results which contain any of the values. To use the Boolean operator AND to search for Tweets with two or more words in them, use two ampersands (*&amp;&amp;*) to separate the two words.
    * For example, entering ** ` Contains any of these words` ** keywords Giants, Posey, and ** ` Does not contain any of these words` ** keyword Dodger, will return all Tweets which include the word *Giants* or *Posey* and do not include the word *Dodger*. 
      To search for Tweets that include both the words *Giants* and *Posey*, enter “Giants &amp;&amp; Posey”. This feature is supported only for the ** ` Contains any of these words` ** and ** ` Does not contain any of these words` ** fields in Twitter rules.


* ** ` Hashtags` **. 
    * Enter ** ` Hashtags` ** to be included in, or excluded from your Twitter stream. Specifying values for both the ** ` Contains any of these words` ** and ** ` Does not contain any of these words` ** fields will return Tweets which contain hashtags in the first field, and do not contain hashtags in the second field. You can enter multiple values for a single field. The stream returns results which contain any of the values.

* ** ` Usernames` ** 
    * Enter ** ` @mentions` ** or ** ` authors` ** to pull into the stream, or exclude from the stream. Use the checkboxes to define whether ** ` Retweets` ** or ** ` replies` ** from selected authors should also be included.

      >[!NOTE]
      >
      >You may either include or exclude authors; you cannot combine these two fields into a single Twitter Rule.


* ** ` Minimum number of followers.` ** Select the minimum number of followers the user must have to pull information from their posts.
* ** ` Location` ** 
    * Enter the location (city, zipcode, address, or geocode in the common latitude/longitude format (+/- 90, +/- 180) ). Begin typing a location to display a drop down menu with suggestions. Select a location from the drop down. The map displays a pin of that location. Adjust the slider to select a radius of one mile to 25 miles for each location. If you do not choose a radius, Livefyre automatically chooses a default of eight miles.

      >[!NOTE]
      >
      >For both fields, distance will be calculated from the center of the input location.

    * You can add more than one location and radius. You can delete a location by clicking the X next to the name of a location in the box.

    * Combine the ** ` Is near this location` ** and ** ` Is not near this location` ** fields to pull content within locations in the ** ` Is near this location` ** field, but not near the locations in the ** ` Is not near this location` ** field.


* ** ` Additional Filters` ** 
    * Use Additional Filters to further refine your Twitter Rule. Define whether you will:     
        * Include ** ` Replies` ** to the targeted Tweets (If the stream becomes high velocity, this feature will automatically be disabled.).
        * Include Tweets from ** ` Verified Twitter accounts only.` **
        * Include ** ` All Content` **, or ** ` Vines Only` **, or ** ` Images Only.` **
        * Include only Tweets which originate from accounts with the selected ** ` Minimum number of followers` ** (any, 100, 500, 1000, 10,000, or 100,000).


For additional Stream rule options for all Stream rules, see [ Stream Rule Options for All Stream Rules ](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules). 
