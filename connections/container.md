# Container

Containers are in essence your own Virtual Private Servers run invisibly in the background of Codeanywhere, each one with its own amount of RAM, Disk space and Processing power. Containers give you the ability to provision any Development Environment you like. You can even choose between one of the predefined stacks:

- Blank – Blank Development Box
- PHP – PHP Development Box with Apache, PHP, MySQL, phpMyAdmin and Composer preinstalled
- NodeJS – NodeJS Development Box with NodeJS, MySQL, NPM, bower and grunt preinstalled
- Ruby – Ruby Development Box with RVM and Ruby on Rails preinstalled
- Python – Python Development Box with pip and virtualenv preinstalled
- C/C++ – C/C++ Development Box with gcc and g++ compiler and gdb preinstalled
- HTML – HTML5 Development Box with Apache, npm, yeoman, bower and  grunt preinstalled
- Wordpress – PHP Development  Box with Wordpress 4.2.1, Apache, PHP, MySQL, phpMyAdmin and Composer preinstalled
- Laravel – PHP Development Box with Laravel 4.2, Apache, PHP, MySQL, phpMyAdmin and Composer preinstalled
- MEAN – NodeJS Development Box with MEAN 0.9.20, NodeJS, bower, MongoDB, gulp and grunt preinstalled
- Symfony – PHP Development Box with Symfony 2.6, Apache, PHP, MySQL, phpMyAdmin and Composer preinstalled
- Sails – NodeJS Development Box with Meteor, NodeJS, NPM, bower and grunt preinstalled
- Meteor – Meteor Development Box with Meteor, NodeJS, NPM, bower and grunt preinstalled
- EmberJS – EmberJS Development Box with EmberJS, NodeJS, NPM, bower and grunt preinstalled
- ioJS – ioJS Development Box with ioJS, NodeJS, NPM, bower and grunt preinstalled
- BackboneJS – BackboneJS Development Box with BackboneJS, Apache (running on standard HTTP port – 80), NPM, bower, grunt preinstalled
- AngularJS – AngularJS Development Box with NodeJS, MySQL, NPM, bower and grunt preinstalled
- CakePHP – PHP Development Box with Apache (running on standard HTTP port – 80), CakePHP, PHP, MySQL (user: myapp, password: secret), and Composer preinstalled
- Drupal – PHP Development Box with Apache (running on standard HTTP port – 80), Drupal, PHP, MySQL (myapp user secret password), phpMyAdmin and Composer preinstalled
- LoopBack – NodeJS Development Box with LoopBack, NodeJS, MySQL, NPM, bower and grunt preinstalled

You won't even be aware of it being created or started. You can choose between two operating systems: Ubuntu and CentOS.

![container-create](images/container-create.png "container-create")


Also, if you require any development environment you can't find in our list, you can use your SSH terminal and create your own stack! Afterwards, just save it as a Custom Stack and you can use it again and again!
The best part of Containers is that not only does it remove issue of having your development environment wherever you are; it also enables you to connect to any GIT repository in the world, be it a corporate server or popular services like GitHub or Bitbucket. With Containers you can now finally connect to your repositories and use its full capabilities, so now you can use commit to repositories from Codeanywhere!

Create a new Container by going to File -> New Connection -> Container

![container-open](images/container-open.png "container-open")

Choose your environment, name it and click Create!

![container-php](images/container-php.png "container-php")

With containers, you can view your code with your preview link. You can check your preview link inside Info with a right click on your Container:
 
![phpinfo](images/phpinfo.png "phpinfo")


When your info tab is opened, use the link at the bottom of your page to access applications running on your Container (see the example below). Be sure to replace the XX with the port you have specified in your app.
 
 ### PHPMyAdmin

PhpMyAdmin comes preinstalled with our Containers (both CentOS and Ubuntu). To access it first open the info by right-clicking the Container in File Explorer:
Copy the link (with the XX replaced with your port) into the new tab of your browser and add „/phpmyadmin“ at the end of the link to access phpMyAdmin – it will look something like: http://port-80.xxxxxx.box.codeanywhere.com/phpmyadmin. For login use the "root" as Username, and leave the Password field empty:
 
![phppmyadmin](images/phpmyadmin.png "phppmyadmin")


If you want to be able to access your Container at all times, you can activate our feature Always-on, which will keep your Container running even when you're not using Codeanywhere!

### Deploy to Heroku

Deploying with Heroku requires you to install Heroku toolbelt. You can install it using SSH command:

```sh	
	wget -O- https://toolbelt.heroku.com/install-ubuntu.sh | sh
```

Now you can use Heroku CLI. More detailed instruction can be found on official Heroku toolbelt website https://toolbelt.heroku.com/


### Locate Private and Public key of a Container

You can view Private Key of your container by going to cd /home/cabox/.ssh/ using your SSH terminal. There you will find: 
- id_rsa - private key container of your container, 
- id_rsa.pub - public key of your container.


### How to connect to a Container via SFTP?

These are the credentials you'll need: 
- Hostname: preview link of your container - looks something like preview.xxxx.box.codeanywhere.com and you can check it in Container's Info with a right click on your Container 
- User name: cabox 
- As for the password, you can't connect this way. You'll need private key of your Container and you can get it by going to /home/cabox/.ssh/id_rsa and that's your private key which you can use for connecting to your Container. 
- Also, you'll need to check your Port - right click on your Container, select Info, locate SSH Terminal listening on port, and that's the port you have to use for connecting to SFTP.

Containers are available to all users, just login and try it out!
