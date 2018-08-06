---
description: You can log a user in through the console during integration and testing to debug authorization.
seo-description: You can log a user in through the console during integration and testing to debug authorization.
seo-title: Debugging Auth Delegate
solution: Experience Manager
title: Debugging Auth Delegate
uuid: 10d6e8e9-228a-4b48-be73-5a56d3b073d0
index: y
internal: n
snippet: y
translate: y
---

# Debugging Auth Delegate

Log a user in through the console using the following ` auth.authenticate` (token) and pass a Livefyre user token to authenticate users on the page.
You may also modify the example shown above, and add the following snippet in-line in your JavaScript to quickly log a user into Livefyre (requires a reference to auth).

```
window.addEventListener('userAuthenticated', function(data) { 
 Livefyre.require(['auth'], function (auth) { 
  auth.authenticate({livefyre: data.token}); 
 }); 
});
```
