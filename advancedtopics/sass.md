---
current_menu: sass
---

# Installing SASS

Sass is an extension of CSS that adds power and elegance to the basic language. It allows you to use variables, nested rules, mixins, inline imports, and more, all with a fully CSS-compatible syntax. 

Our [Containers](http://docs.codeanywhere.com/connections/container.html) don't have SASS preinstalled, but you can set it up easily!

First of all, you'll have to create a Container. Of course, you can use any Stack, but you'll have to install Ruby first. 
In order to install Ruby, use:
```sh
sudo apt-get install ruby-full
```
on Ubuntu, or:
```sh
sudo yum install ruby 
```
on CentOS.


Now, you just have to install the Sass gem with the following command:
```sh
sudo gem install sass
```

You can use the command line to run Sass:
```sh
sass input.scss output.css
```
