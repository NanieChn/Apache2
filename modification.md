**MODIFICATION**
-
How to transfer my site to server ?
```
root@debian: vim sites-available/000-default.conf
```
On
```
DocumentRoot|
```
Tap this for change
```
c
```
After this for the end of line
```
$
```
Edit
```
DocumentRoot /home/username/mysite
```
*mysite* content your code.

To save 
```
echap
```
```
:x
```
To reload our configuration
```
root@debian: service apache2 reload
```
