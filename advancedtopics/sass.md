---
current_menu: sass
---

# Installing SASS

Sass is an extension of CSS that adds power and elegance to the basic language. It allows you to use variables, nested rules, mixins, inline imports, and more, all with a fully CSS-compatible syntax. 

Our [Containers](http://docs.codeanywhere.com/connections/container.html) don't have SASS preinstalled, but you can set it up easily!

First of all, you'll have to create an Container. Of course, you can use any Stack but you'll have to install Ruby first. The recommended way is to use RVM.
As a first step install [mpapis](https://rvm.io/authors/mpapis/) [public key](https://keybase.io/mpapis) used to verify installation package to ensure security.:
```sh 
gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3 7D2BAF1CF37B13E2069D6956105BD0E739499BDB
```
Install RVM stable with ruby:
```sh 
curl -sSL https://get.rvm.io | bash -s stable --ruby
```
Now you may load RVM with the following command:
```sh
source ~/.rvm/scripts/rvm
```

Now, you just have to install the Sass gem with the following command:
```sh
gem install sass
```

You can use command line to run Sass, just use
```sh
sass input.scss output.css
```
