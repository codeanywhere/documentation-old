---
current_menu: container
---

# Container

Containers are like your own Virtual Private Servers (in essence they are OpenVZ OS containers) provisioned by Codeanywhere, each one with its own amount of RAM, Disk space and Processing power (just like any normal VPS but with some limitations such as lack of a dedicated IP address). Containers give you the ability to provision any Development Environment you like. You can choose between one of the predefined stacks:

- Default – Blank Development Container
- PHP – LAMP Development Stack with phpMyAdmin and Composer preinstalled
- NodeJS – NodeJS Development Stack with npm and yarn preinstalled
- Ruby – Ruby Development Stack with RVM and Ruby on Rails preinstalled
- Python – Python Development Stack with pyenv, pip and virtualenv preinstalled
- C/C++ – C/C++ Development Stack with gcc and g++ compiler and gdb preinstalled
- HTML – HTML5 Development Stack with Apache, Node.js and npm preinstalled
- Wordpress – LAMP Development Stack with Wordpress, phpMyAdmin and Composer preinstalled
- Java – Java Development Stack with OpenJDK7, OpenJDE7 and Tomcat7 preinstalled
- .NET Core – .NET Core Development Stack


You won't even be aware of it being created or started. You can choose between two operating systems: Ubuntu 16.04 and CentOS 7.2.

![container-create](images/container-create.png "container-create")


Also, if you require any development environment you can't find in our list, you can create a container from a Blank stack and install anything you want and you can find some popular stacks installation steps in our Advanced Topics section. Afterwards, just save it as a Custom Stack and you can use it again and again!
The best part of Containers is that not only does it remove issue of having your development environment wherever you are; it also enables you to connect to any GIT repository in the world, be it a corporate server or popular services like GitHub or Bitbucket. With Containers you can now finally connect to your repositories and use its full capabilities, so now you can use commit to repositories from Codeanywhere!

Create a new Container by going to File -> New Connection -> Container

![container-open](images/container-open.png "container-open")

Choose your environment, name it and click Create!

![container-php](images/container-php.png "container-php")

### Manage Container

<img src="images/container-manage.png" width="200" height="auto">


With Container get SSH access to your Container and you can use all the necessary actions such as git commands, installation of new depencencies ect! You can Turn Off or Turn On your Box, restart it or set it to be Always On so you can access your Box at anytime, without the need of logging into your account and starting it.
With containers, you can view your code with your preview link. You can check your preview link inside Info.
 
![phpinfo](images/container-info.png "container-info")

Be sure to replace the XX with the port you have specified in your app.

In Config, you can set up commands necessary for your Stack to Run. Custom Stack can be created out of any Container! If you installed anything using your terminal, just save it as a Custom Stack and use it again and again. This way, you don't have to lose anytime for creating your development environment all over again!

By selecting Run, your preview link will be opened and any command neccessary to run your app, opened in SSH terminal.

Create any file, by entering filename.extension, or folder inside your container, Upload files directly from your local storage or Share your entire Container!
 
In case you want to delete your entire Container, just click Destroy. However, keep in mind that your work will be removed and you wont be able to retrieve it afterwards!


### Creating a Custom Stack

In order to create a Custom Stack of one of your Stacks, first, you'll have to right click on your Container and select Create Custom Stacks

<img src="images/ccs1.png" width="200" height="auto">

Enter your File name and Description so you could find it easier later on!

![ccs2](images/ccs2.png "ccs2")

You can access all your Custom Stacks in your [Dashboard](https://codeanywhere.com/dashboard#custom-stacks).


### Deploy to Heroku

Deploying with Heroku requires you to install Heroku toolbelt. You can install it using SSH command:

```sh	
	wget -O- https://toolbelt.heroku.com/install-ubuntu.sh | sh
```

Now you can use Heroku CLI. More detailed instruction can be found on official Heroku toolbelt website https://toolbelt.heroku.com/


### Locate Private and Public

You can view Keys of your container by going to cd /home/cabox/.ssh/ using your SSH terminal. There you will find: 
- id_rsa - private key container of your container, 
- id_rsa.pub - public key of your container.


### Connect your Container via SSH

![containerhostname](images/container-hostname.png "container-hostname")

These are the credentials you'll need: 
- Hostname and port: check it in Container's Info with a right click on your Container, select Info, locate SSH access, and that's the hostname and port you have to use.
- User name: cabox 
- As for the password, you can't connect this way. You'll need private key of your Container and you can get it by going to /home/cabox/.ssh/id_rsa and that's your private key which you can use for connecting to your Container.

Containers are available to all users, just login and try it out!