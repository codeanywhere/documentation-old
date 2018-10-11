---
current_menu: angular
---

# Installing Angular framework

In order to install Angular framework, first create a [Container](http://docs.codeanywhere.com/connections/container.html) with the Node.js stack. Node.js has it's own package manager `npm` with whom you will install the Angular CLI.

```sh
$ npm install -g @angular/cli
```
Now that you have the Angular CLI installed, create a new project in your `workspace`:
```sh
$ cd ~
$ ng new workspace 
```
After the project is created, go to the project directory and launch the server:
```sh
$ cd ~/workspace
$ ng serve --host 0.0.0.0 --port 3000
```

Once launched, you can preview your application with your container preview URL.