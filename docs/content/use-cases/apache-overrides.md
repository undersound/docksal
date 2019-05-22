---
title: "Overriding Apache with Advanced Virtual Host Settings"
weight: 1
---

Simulating a remote server configuration in local development may mean more advanced virtual host settings. 
Use `.docksal/etc/apache/httpd-vhost-overrides.conf` to override the default virtual host configurations.

```
<Directory "/var/www/common/">
    Require all granted
</Directory>

Alias /resources/ "/var/www/common/"


<Directory "/var/www/docroot/">
   DirectoryIndex index.php
</Directory>

<Directory "/var/www/docroot">
   DirectoryIndex index.php

   <IfModule mod_rewrite.c>
      RewriteEngine on
      RewriteRule ^$ /resources/framework/index.php [L]
      RewriteCond %{REQUEST_FILENAME} !-f
      RewriteCond %{REQUEST_FILENAME} !-d
      RewriteRule ^(.*)$ /resources/framework/index.php?q=$1 [QSA,PT]
   </IfModule>

</Directory>

```