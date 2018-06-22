---
description: Create a Network object.
seo-description: Create a Network object.
seo-title: Network Class Methods
solution: Experience Manager
title: Network Class Methods
---

# Network Class Methods

Once you create a network object, the rest of the page will assume that you have a instantiated Network object in your session.

<table frame="all" rowsep="1" colsep="1" id="table_lyk_dzs_kbb"> 
 <title>Network Object</title> 
 <tgroup cols="3"> 
  <colspec colname="c1" colnum="1" colwidth="1.0*" /> 
  <colspec colname="c2" colnum="2" colwidth="1.0*" /> 
  <colspec colname="c3" colnum="3" colwidth="1.0*" /> 
  <thead> 
   <tr> 
    <th class="entry"> Parameter </th> 
    <th class="entry"> Type </th> 
    <th class="entry"> Description </th> 
   </tr> 
  </thead> 
  <tbody> 
   <tr> 
    <td> <span class="varname"> network </span> </td> 
    <td> String </td> 
    <td> Your Livefyre network. For example: “labs.fyre.co”. </td> 
   </tr> 
   <tr> 
    <td> <span class="varname"> networkKey </span> </td> 
    <td> String </td> 
    <td> The Livefyre-provided secret key for the network. </td> 
   </tr> 
  </tbody> 
 </tgroup> 
</table>

## Java {#section_myk_dzs_kbb}

```
import com.livefyre.Livefyre; 
 
Network network = Livefyre.getNetwork(network, networkKey); 

```
## NodeJS {#section_nyk_dzs_kbb}

```
var livefyre = require('livefyre'); 
 
var network = livefyre.getNetwork(network, networkKey); 

```
## PHP {#section_oyk_dzs_kbb}

```
use Livefyre\Livefyre; 
 
$network = Livefyre::getNetwork(network, networkKey); 

```
## Python {#section_pyk_dzs_kbb}

```
from livefyre import Livefyre 
 
network = Livefyre.get_network(network, networkKey) 

```
## Ruby {#section_qyk_dzs_kbb}

```
require 'livefyre' 
 
network = Livefyre.get_network(network, networkKey) 

```
