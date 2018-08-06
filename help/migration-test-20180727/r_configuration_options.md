---
description: The Sidenotes config object is a JSON object used to specify the content that the Livefyre App renders on the page.
seo-description: The Sidenotes config object is a JSON object used to specify the content that the Livefyre App renders on the page.
seo-title: Sidenotes Configuration Options
solution: Experience Manager
title: Sidenotes Configuration Options
uuid: d4e4360f-1432-44dd-a745-a413ed0a028e
index: y
internal: n
snippet: y
translate: y
---

# Sidenotes Configuration Options




The object contains the following parameters:

<table frame="all" rowsep="1" colsep="1" id="table_rfj_cmj_yy"> 
 <thead> 
  <tr> 
   <th class="entry">Parameter</th> 
   <th class="entry">Type</th> 
   <th class="entry">Description</th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td>authDelegate</td> 
   <td>(required) object</td> 
   <td>New or old style initialized authentication delegate.</td> 
  </tr> 
  <tr> 
   <td>collectionMeta</td> 
   <td>(required) object</td> 
   <td>See collectionMeta token for more information.</td> 
  </tr> 
  <tr> 
   <td>customIcon</td> 
   <td>(optional) string</td> 
   <td>Sets the URL of a custom launcher icon. Defaults to Livefyre bubble.</td> 
  </tr> 
  <tr> 
   <td>customStyles</td> 
   <td>(optional) object</td> 
   <td>Adds custom styles to change the look and feel of Sidenotes. For more information, see Custom Styles.</td> 
  </tr> 
  <tr> 
   <td>disableStream</td> 
   <td>(optional) Boolean</td> 
   <td>If true, disables real-time streaming in this Sidenotes instance (not in other comment streams). Default is false.</td> 
  </tr> 
  <tr> 
   <td>environment</td> 
   <td>(optional) string</td> 
   <td>Specifies the Livefyre UAT environment. The only possible value is t402.livefyre.com. For production this parameter must be removed.</td> 
  </tr> 
  <tr> 
   <td>iconVisibility</td> 
   <td>(optional) object or string</td> 
   <td>Defines whether the Sidenotes icon will be visible upon hover or static. If this is a string, it will be used for both versions of the block icon (empty and has Sidenotes). If an object, you must specify each type: {empty: ‘hover’, num: ‘static’}. Default is static.</td> 
  </tr> 
  <tr> 
   <td>inlineThreads</td> 
   <td>(optional) Boolean</td> 
   <td>If true, Sidenote threads are inserted directly after the block with which they are associated. Default is false.</td> 
  </tr> 
  <tr> 
   <td>numSidenotesEl</td> 
   <td>(optional) object, string, or array</td> 
   <td> <p>Specifies which element the Sidenotes count widget will decorate. (This widget shows the number of sidenotes on the page and information about Sidenotes.)</p> <p>If the string selector matches more than one element, the first will be chosen. (Uses CSS3 DOM selector spec.)</p> </td> 
  </tr> 
  <tr> 
   <td>position</td> 
   <td>(optional) string</td> 
   <td>Determines the position of the popup when an element that has Sidenotes enabled is clicked. Possible values are ‘smart’, ‘left’, ‘right’, ‘bottom’. Default is ‘smart’ which aligns the popup to the right of the page unless there is not enough space (in which case it will move to below the content).</td> 
  </tr> 
  <tr> 
   <td>selectors</td> 
   <td>(required) object, string, or array</td> 
   <td> <p>Specifies the elements on which launcher icons should appear. (Uses CSS3 DOM selector spec.)</p> <p>If object, includes an “includes” section and an “excludes” section that will apply the CSS selector for any matching includes, and remove any elements matching the excludes. If string, will include any matching elements on the page. If array, lists the elements to include.</p> </td> 
  </tr> 
  <tr> 
   <td>strings</td> 
   <td>(optional) object</td> 
   <td>Adds custom text strings to change any language or text throughout the application. For more information, see Custom Strings.</td> 
  </tr> 
  <tr> 
   <td>threadContainerEl</td> 
   <td>(optional) object, string, or array</td> 
   <td> <p>Specifies an element where the thread of sidenotes will appear. This parameter allows you to reposition the thread.</p> <p>If the string selector matches more than one element, the first will be chosen. (Uses CSS3 DOM selector spec.)</p> </td> 
  </tr> 
 </tbody> 
</table>

