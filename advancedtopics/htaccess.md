---
current_menu: htaccess
---


### .htaccess

CWD (curent working directory) - inside your Config file - is the location in which your run commands should be located. The default location is ~/workspace, if your commands are located in a subdirectory named "test” then cwd should be ~/workspace/test.

Apache installed on containers by default usually point to the workspace directory for the root of the website. If you need it to point elsewhere create or edit the .htaccess file located in the workspace directory. 
Here are the instructions for you: 
```sh
vim .htaccess 
```
```sh
<IfModule mod_rewrite.c> 
RewriteEngine on 
RewriteRule ^(.*)$ directory-name/$1 [L] 
</IfModule>
```

The directory “directory-name” should be a subdirectory of workspace. Example: ~/workspace/test/test2/last-try/index.html 
RewriteRule ^(.*)$ test/test2/last-try/$1 [L]