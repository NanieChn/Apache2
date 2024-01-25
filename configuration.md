**CONFIGURATION**
-
<span style="color:green">To see for what port Apache2 is running</span>
```
vim /etc/apache2/apache2.conf
```
```
/listen
```
There is *ports.conf*
```
:q!
```
```
vim /etc/apache2/ports.conf
```
There is *Listen 80* and that's means 80 is the port for what Apache is running by default.

<span style="color:green">Then</span>
```
cd /etc/apache2/
```
```
ls -la
```
There is *sites-available* and *sites-enabled*
```
ls sites-available/
```
There is *000-default.conf* and *default-ssl.conf*. *000-default.conf* is the configuration of the site by default and *000* means that this configuration must be loaded first.
```
ls sites-enabled/ -l
```
There is just a *symlink* to sites-available

When we'll make our own configuration in the *sites-available* and if we need to activate or desactivate the site, just activate or desactivate the *symlink* for avoid the loss of configuration because we delete nothing.

<span style="color:green">Next</span>
```
vi sites-enabled/000-default.conf
```
There is */var/www/html*
```
ls /var/www/html
```
There is *index.html*
```
vim /var/www/html/index.html
```
There is our <span style="color:yellow">HTML code</span>.
