**ERROR**
-
If you see an error when you try to verify your site on browser.
```
root@debian: ls -la /var/log/apache2/
```
There is *error.log*
```
root@debian: tail -n 30 /var/log/apache2/error.log
```
At the end, it say that Apache 2 can't acces */home/username/mysite/*

On `DocumentRoot|` in *sites-available/000-default.conf* 
```
DocumentRoot /var/www/html
```
Reload and verify on browser because you should see that Apache 2 can't access all files so if we need to create a new file, modify *apache2.conf*

help 
```
/etc/apache2/usr/sbin/apache2ctl configtest
```



