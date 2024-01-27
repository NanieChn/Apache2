**SOLUTION**
-
Go back with
```
DocumentRoot /home/username/mysite
```
```
root@debian: vim apache2.conf
```
```
/var\/www
```
Add
```
<Directory /home/username/mysite>
    Options FollowSymLinks
    AllowOverride None
    Require all granted
</Directory>
```
Save, reload and verify on browser.
This method require a modification for *apache2.conf*
