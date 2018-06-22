---
description: Installing the libraries for Livefyre server-side tasks
seo-description: Installing the libraries for Livefyre server-side tasks
seo-title: Installation
solution: Experience Manager
title: Installation
---

# Installation


>## Installation {#c_installing_libraries}
>Installing the libraries for Livefyre server-side tasks

<!-- c_installing_libraries.dita -->
## Java {#section_yd3_3zk_rz}

To install the Java library, add this dependency to your project’s POM:

```
&lt;dependency&gt; 
 &lt;groupId&gt;com.livefyre&lt;/groupId&gt; 
 &lt;artifactId&gt;livefyre&lt;/artifactId&gt; 
 &lt;version&gt;2.0.3&lt;/version&gt; 
&lt;/dependency&gt;
```
The Java library has dependencies on the following modules:

```
&lt;dependency&gt; 
 &lt;groupId&gt;com.sun.jersey&lt;/groupId&gt; 
 &lt;artifactId&gt;jersey-client&lt;/artifactId&gt; 
 &lt;version&gt;[1.18.1,)&lt;/version&gt; 
&lt;/dependency&gt; 
&lt;dependency&gt; 
 &lt;groupId&gt;com.google.code.gson&lt;/groupId&gt; 
 &lt;artifactId&gt;gson&lt;/artifactId&gt; 
 &lt;version&gt;[2.3,)&lt;/version&gt; 
&lt;/dependency&gt; 
&lt;dependency&gt; 
 &lt;groupId&gt;com.google.guava&lt;/groupId&gt; 
 &lt;artifactId&gt;guava&lt;/artifactId&gt; 
 &lt;version&gt;[18.0,)&lt;/version&gt; 
&lt;/dependency&gt; 
&lt;dependency&gt; 
 &lt;groupId&gt;org.apache.commons&lt;/groupId&gt; 
 &lt;artifactId&gt;commons-lang3&lt;/artifactId&gt; 
 &lt;version&gt;[3.0.1,)&lt;/version&gt; 
&lt;/dependency&gt; 
&lt;dependency&gt; 
 &lt;groupId&gt;org.bitbucket.b_c&lt;/groupId&gt; 
 &lt;artifactId&gt;jose4j&lt;/artifactId&gt; 
 &lt;version&gt;[0.4.1,)&lt;/version&gt; 
&lt;/dependency&gt; 

```
<a id="section_rlh_qys_kbb"></a>

For more information, read the Java docs or see the source on [ GitHub ](https://github.com/Livefyre/livefyre-java-utils).

## NodeJS {#section_swj_pwq_rz}

To install the NodeJS library, run this line:

```
$ npm install livefyre 

```
The NodeJS library has dependencies on the following modules:

```
"restler":"&gt;=3.2.0", 
"validator":"=3.5.0", 
"jsonwebtoken": "&gt;=5.0.0" 

```
For more information, read the NodeJs docs or see the source on [ GitHub ](https://github.com/Livefyre/livefyre-nodejs-utils).

Links: [ Restler ](https://github.com/danwrong/restler), [ Validator ](https://www.npmjs.org/package/validator), [ jsonwebtoken ](https://github.com/auth0/node-jsonwebtoken).

## PHP {#section_txj_xwq_rz}

To install the PHP library with Composer, add this to your composer.json:

```
"require": { 
 "livefyre/livefyre-php-utils": "2.0.4" 
}
```
Then install using:

```
composer.phar install 

```
If you do **not** use Composer, obtain the latest version of the library using:

```
git clone https://github.com/Livefyre/livefyre-php-utils 

```
To use the library, add the following to your PHP script:

```
require_once("/path/to/livefyre-php-utils/src/Livefyre.php"); 

```
The PHP library has dependencies on the following modules:

```
"ext-json": "*", 
"rmccue/requests": "&gt;=1.0" 
"firebase/php-jwt": "&gt;=2.0" 

```
For more information, read the PHP docs or see the source on [ GitHub ](https://github.com/Livefyre/livefyre-php-utils).

Links: [ ext-json ](https://php.net/manual/en/book.json.php), [ Requests ](https://github.com/rmccue/Requests/), [ PHP-JWT ](https://github.com/firebase/php-jwt/tree/v2.0.0)

## Python {#section_irk_fxq_rz}

To install the Python library, run this line:

```
$ pip install livefyre 

```


The Python library has dependencies on the following modules:

```
PyJWT &gt;= 1.0.1 
requests &gt;= 2.2.1 
python-dateutil &gt;= 2.2 
enum34 == 1.0 
ordereddict == 1.1 if sys.version_info[:2] &lt; 2.7 

```
For more information, read the Python docs or see the source on [ GitHub ](https://github.com/Livefyre/livefyre-python-utils).

Links: [ PyJWT ](https://github.com/progrium/pyjwt), [ Requests ](https://github.com/kennethreitz/requests), [ Python-Dateutil ](https://pypi.python.org/pypi/python-dateutil), [ Enum34 ](https://pypi.python.org/pypi/enum34), [ OrderedDict ](https://pypi.python.org/pypi/ordereddict)

## Ruby {#section_fv2_tzq_rz}

To install the Ruby library, add this line to your application’s Gemfile:

```
gem 'livefyre' 

```
Or install it yourself:

```
$ gem install livefyre 

```


The Ruby library has dependencies on the following modules:

```
"jwt", '~&gt; 1.4', "&gt;= 1.4.1" 
"rest-client", '~&gt; 1.8', "&gt;= 1.8.0" 
"addressable", '~&gt; 2.3', "&gt;= 2.3.6" 

```
For more information, read the Ruby docs or see the source on [ GitHub ](https://github.com/Livefyre/livefyre-ruby-utils).

Links: [ Ruby JWT ](https://github.com/firebase/php-jwt/tree/v2.0.0), [ REST Client ](https://github.com/rest-client/rest-client/), [ Addressable ](https://github.com/sporkmonger/addressable)

