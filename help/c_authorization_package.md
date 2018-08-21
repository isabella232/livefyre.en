---
description: Install the Authentication Package to enable user authentication so users can interact with your apps.
seo-description: Install the Authentication Package to enable user authentication so users can interact with your apps.
seo-title: Authentication Package
solution: Experience Manager
title: Authentication Package
uuid: d2faf9ce-0e09-4ff0-8895-d53c4ddefd4f
index: y
internal: n
snippet: y
translate: y
---

# Authentication Package

Livefyre Apps use the global auth package to associate users with App actions. The auth package is available through ` Livefyre.require`.

To enable authentication on your page, first add ` Livefyre.js` to the ` <head>` element of your webpage or website template.

```
<script src="//cdn.livefyre.com/Livefyre.js"></script>
```
Using Livefyre.require to enable auth is similar to using require to call other packages. The integration code to require auth looks like this:

```
Livefyre.require(['auth'], function (auth) {  
// Perform action... 
});
```

## Methods {#section_ojx_1lz_fz}

Once included as above using ` Livefyre.require`, the Auth module exposes the following methods that you can call to notify other Apps on the page about authentication-related events.

#### Methods
<table frame="all" rowsep="1" colsep="1" id="table_zlx_1mz_fz">  
 <thead> 
  <tr> 
   <th class="entry"> Method </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td> <span class="codeph"> .login(callback) </span> </td> 
   <td> Trigger the login flow as implemented by the registered AuthDelegate. Usually only auth-enabled Apps will call this, and not the host page itself. </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> .logout(callback) </span> </td> 
   <td> Notify auth that the end-user has logged out by some external means, and that all relying Apps should clear their authentication state until the next login. This will clear the internal session maintained by Auth. </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> .authenticate(credentials) </span> </td> 
   <td> <p>Notify Auth that a user has authenticated by some external means, and a Livefyre Authentication Token has been procured for the end-user. Use this if you set a cookie with the Livefyre token, or have a token for the user and want to explicitly log the user in. For example: 
     <codeblock>
       auth.authenticate({&amp;nbsp;livefyre:&amp;nbsp;'&amp;lt;insert&amp;nbsp;lftoken&amp;nbsp;string&amp;nbsp;for&amp;nbsp;newly&amp;nbsp;logged-in&amp;nbsp;user&amp;gt;'&amp;nbsp;}); 
     </codeblock></p> </td> 
  </tr> 
  <tr> 
   <td> <span class="codeph"> .delegate(authDelegate) </span> </td> 
   <td> Delegate the implementation details of authentication (for example, your custom authentication flow) to an object that you define. This must be called by the host page to enable interactive features of Livefyre Apps. </td> 
  </tr> 
 </tbody> 
</table>

