Hello World Example <requires>PHP >= 5.3</requires>
-------------------

<tag>basic</tag>

Basic hello world example to get started with Restler 3.

> This API Server is made using the following php files/folders

> * index.php      (gateway)
> * Say.php      (api)
> * restler.php      (framework)
> * JsonFormat.php      (format)

This API Server exposes the following URIs

    GET say/hello   ⇠ Say::hello()
    GET say/hi/{to} ⇠ Say::hi()


> **Note:-** If you have used Restler 2 before you will wonder why
 the generated routes are lesser with Restler 3.
 Read the [Routes](../_006_routing/readme.html) example to understand.



Try the following links in your browser

GET [say/hello](say/hello)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hello world!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

GET [say/hello?to=R.Arul%20Kumaran](say/hello?to=R.Arul%20Kumaran)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hello R.Arul Kumaran!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

GET [say/hi/restler3.0](say/hi/restler3.0)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hi restler3.0!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


If the above links fail, it could be due to missing `.htaccess` file or URL Rewriting is not supported in your server.
Try the following links instead

GET [index.php/say/hello](index.php/say/hello)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hello world!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

GET [index.php/say/hello?to=R.Arul%20Kumaran](index.php/say/hello?to=R.Arul%20Kumaran)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hello R.Arul Kumaran!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

GET [index.php/say/hi/restler3.0](index.php/say/hi/restler3.0)
:    
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
"Hi restler3.0!"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



*[index.php]: _001_helloworld/index.php
*[Say.php]: _001_helloworld/Say.php
*[restler.php]: ../../vendor/restler.php
*[JsonFormat.php]: ../../vendor/Luracast/Restler/Format/JsonFormat.php