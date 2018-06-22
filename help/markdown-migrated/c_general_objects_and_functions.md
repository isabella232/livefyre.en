---
description: Use Javascript to customize your Livefyre instance.
seo-description: Use Javascript to customize your Livefyre instance.
seo-title: Customize Livefyre with Objects, Tokens, and Functions
title: Customize Livefyre with Objects, Tokens, and Functions
---

# Customize Livefyre with Objects, Tokens, and Functions

Livefyre provides the following functions:

* Auth.delgate function
* livefyre.require function
You must set up the following JSON Web Tokens (JWT's) to use the functions and objects:

* userAuth token
* collectionMeta token
The following objects apply to all Livefyre Apps and must be set up before you can customize an App using javascript. You use these objects in each instance of an App customization:

  *
  AuthDelegate
  
  
  *
  CollectionMeta
  
  
  *
  ConvConfig
  
  
  *
  NetworkConfig
  
  
For each App, you must specify additional parameters for the following objects:

  *
  ConvConfig
  
  
  *
  NetworkConfig
  
  
  *
  CollectionMeta
  
  
Some Apps have additional objects and parameters that you must specify in order to use them. See the details about App objects in the App documentation.

