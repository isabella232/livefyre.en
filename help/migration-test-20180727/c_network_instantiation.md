---
description: Create a Network object.
seo-description: Create a Network object.
seo-title: Network Instantiation
title: Network Instantiation
uuid: b0f32ec0-d941-4ca4-8c5f-1e588d175e29
index: y
internal: n
snippet: y
translate: y
---

# Network Instantiation

Once you create a network object, the rest of the page will assume that you have a instantiated Network object in your session.

#### Network Object
|  Parameter  | Type  | Description  |
|---|---|---|
|  * ` network` * | String  | Your Livefyre network. For example: “labs.fyre.co”.  |
|  * ` networkKey` * | String  | The Livefyre-provided secret key for the network.  |


## Java {#section_odb_4jr_rz}


```
import com.livefyre.Livefyre; 
  
Network network = Livefyre.getNetwork(network, networkKey); 

```

## NodeJS {#section_vnt_zjr_rz}


```
var livefyre = require('livefyre'); 
  
var network = livefyre.getNetwork(network, networkKey); 

```

## PHP {#section_e22_bkr_rz}


```
use Livefyre\Livefyre; 
  
$network = Livefyre::getNetwork(network, networkKey); 

```

## Python {#section_zqc_2kr_rz}


```
from livefyre import Livefyre 
  
network = Livefyre.get_network(network, networkKey) 

```

## Ruby {#section_hhb_gkr_rz}


```
require 'livefyre' 
  
network = Livefyre.get_network(network, networkKey) 

```
