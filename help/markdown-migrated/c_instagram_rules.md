---
description: You can create Stream rules that pull content from Instagram.
seo-description: You can create Stream rules that pull content from Instagram.
seo-title: Instagram Rules
title: Instagram Rules
---

# Instagram Rules

>[!NOTE]
>
>Before you create an Instagram stream, you must add at least one corporate Instagram account to the `uicontrol Social Accounts` section in `uicontrol Network Settings`. For more information on how to configure a social account, see Social Accounts.
>
>
Create Instagram Rules based on @mentions, hashtag, or location.

>[!NOTE]
>
>All Instagram rules require at least one hashtag. Adding keywords and a Username for your rule will return content which includes both entries.
To create Instagram Rules to pull content from Instagram feeds into your App or Folder, filter by:

* `uicontrol Words`
    * Enter `uicontrol hashtags` to be included in, or excluded from your Instagram stream. Specifying values for both the `uicontrol Contains` and `uicontrol Does not contain` fields will return images which contain the first, and do not contain the second.
    * For example, entering `uicontrol Contains` keywords Giants, Posey, and `uicontrol Does not contain` keyword Dodger, will return all posts which include the word Giants or Posey, and do not include the word Dodger.
      >[!NOTE]
      >
      >Instagram Rules will return posts which include the listed hashtag in the author’s comments, which may not appear in the stream.
      
  
* `uicontrol Mentions`
    * Enter `uicontrol @mentions` to pull into the stream, or exclude from the stream.
  
* `uicontrol Location.`Choose one of the following:
      *
      `uicontrol Map` location (city, zipcode, address, or geocode in the common latitude/longitude format (+/- 90, +/- 180) ). Begin typing a location to display a drop down menu with suggestions. Select a location from the drop down. The map displays a pin of that location. Adjust the slider to select a radius of one mile to three miles for each location. If you do not choose a radius, Livefyre automatically chooses a default of two miles.
      
      You can add more than one location and radius. You can delete a location by clicking the X next to the name of a location in the box.
      
      Combine the `uicontrol Is near this location` and `uicontrol Is not near this location` fields to pull content within locations in the `uicontrol Is near this location` field, but not near the locations in the `uicontrol Is not near this location` field.
      
      >[!NOTE]
      >
      >For both fields, distance will be calculated from the center of the input location.
      >
      >
      
    * `uicontrol Check In Location`
        * Enter the `uicontrol Instagram Place URL` from Instagram. To find the Instagram Place URL:
            1. Search Instagram for a specific check in location. For example, search in Instagram for “golden gate bridge.”
            1. Select the check in location from the list. For example, select the check in location with the name “Golden Gate Bridge.”
            1. Instagram takes you to the webpage for that check in location. There is a map pointing to the location and Instagram posts that have check-ins there. The URL contains a number. This number is the number to put in the `uicontrol Instagram Place URL` field. For example, for the Golden Gate Bridge check in location, the URL is http://www.instagram.com/explore/locations/16839381/golden-gate-bridge/.
          
      
  
* `uicontrol Additional Filters`
    * Select whether you would like to include `uicontrol All Content`, `uicontrol Videos Only`, or `uicontrol Photos Only` in your stream.
  
For additional Stream rule options for all Stream rules, see [Stream Rule Options for All Stream Rules](c_stream_rule_options_for_all_stream_rules.md#c_stream_rule_options_for_all_stream_rules).

