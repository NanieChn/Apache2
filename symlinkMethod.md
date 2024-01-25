**SYMLINK METHOD**
-
Create a *symlink* in */var/www*
```
root@debian:/etc/apache2 vim sites-available/000-default.conf
```
Change
```
DocumentRoot: /var/www
```
Save, reload and verify on browser. There is  **<span style="font-size: 20px">Index of/</span>** because of this option 
```
<Directory /var/www>
    Options Indexes FollowSymLinks
    AllowOverride None
    Require all granted
</Directory>
```
Consequently, someone can see your file.
```
root@debian:/etc/apache2 ln -s /home/username/mysite /var/www/sitename.fr
```
Go on browser. It's done.
