---
description: Use Javascript to customize your Livefyre instance.
seo-description: Use Javascript to customize your Livefyre instance.
seo-title: Creating Livefyre Tokens in C#
title: Creating Livefyre Tokens in C#
uuid: dcc1ac10-22ee-4f56-b88a-7884e2cb73d6
index: y
internal: n
snippet: y
translate: y
---

# Creating Livefyre Tokens in C#

## Creating Livefyre Tokens in C# {#c_general_objects_and_functions}Use Javascript to customize your Livefyre instance.<!-- c_general_objects_and_functions.dita --> Livefyre provides the following functions:

* Auth.delgate function
* livefyre.require function
You must set up the following JSON Web Tokens (JWT's) to use the functions and objects:

* userAuth token
* collectionMeta token
The following objects apply to all Livefyre Apps and must be set up before you can customize an App using javascript. You use these objects in each instance of an App customization:

* AuthDelegate

* CollectionMeta

* ConvConfig

* NetworkConfig

For each App, you must specify additional parameters for the following objects:

* ConvConfig

* NetworkConfig

* CollectionMeta

Some Apps have additional objects and parameters that you must specify in order to use them. See the details about App objects in the App documentation.
>## AuthDelegate Object {#c_building_an_auth_delegate}The 
<codeph>
  AuthDelegate 
</codeph> object implements your desired behavior for how to perform authentication actions and events so you can customize integration with your site’s existing authentication system.<!-- c_building_an_auth_delegate.dita --> 
## Building an Auth Delegate {#section_wmn_tv2_gz}

The auth package must be provided with an auth delegate before it can perform an action. An auth delegate is any JavaScript object that implements one of the methods in this topic.

## .login(finishLogin) {#section_mpk_lv2_gz}

Log in a valid user and invoke the finishLogin function with either an Error object if there was an error, or the user’s Livefyre credentials. Common implementations of this method redirect the user to a login page or open a new window or modal.
This example automatically notifies auth of a Livefyre user with the authentication token, token:

```
authDelegate.login = function (finishLogin) { 
 finishLogin(null, { 
   livefyre: 'token' 
 }); 
};
```
The simplest login delegate might ask the end-user for their Livefyre Authentication token.

```
authDelegate.login = function contrivedLogin(finishLogin) { 
  var lfToken = prompt("Please type your Livefyre Token");  
  if (lfToken.length === 0) { 
   return finishLogin(new Error("User failed to type their lftoken")); 
  }  
 finishLogin(null, { 
   livefyre: lfToken 
 }); 
};
```

## .logout(finishLogout) {#section_uqz_2v2_gz}

Log out a user and invoke the finishLogout function with either an Error object if there was an error, or null to notify auth that the logout was successful.
For example:

```
authDelegate.logout = function (finishLogout) { 
 clearUserSession(); //logic to clear a user session  
 finishLogout(null); 
}
```

## .viewProfile(user) {#section_kkv_dv2_gz}

Take action to view a user’s profile.

```
authDelegate.viewProfile = function (user) { 
 window.open(user.get('profileUrl')); 
}
```

## .editProfile(user) {#section_bkx_pq2_gz}

Take action to edit a user’s profile.

```
authDelegate.editProfile = function (user) { 
 window.open(user.get('profileUrl') + '/edit/'); 
}
```
By implementing all of the methods listed above, auth can be configured with a custom auth delegate. Once a delegate has been constructed, it can be provided to auth using the delegate method.

```
var authDelegate = { 
 login: function(cb) { 
  ... 
  cb(null); 
 }, 
 ... 
} 
  
auth.delegate(authDelegate);
```
