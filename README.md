MODX Evolution Custom htaccess
=========================

MODx Evolution custom htaccess files for better protection 

# What it does

* Send 403 (FORBIDDEN) in response to malicious scripts and bad bots

thanks to mrhaw: https://github.com/mrhaw


# Install

* extract and upload to the root of your MODx Evolution
* rename both ht.access files (one in site root and the other in assets folder) to .htaccess

# Known issues with MODX extras and possible solutions

###multiTV

Create a *.htaccess* file in *assets/tvs/multitv* with the content
```
<files multitv.connector.php>
   Order deny,allow
   allow from all
</filesmatch>
````
