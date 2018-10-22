---
current_menu: meteor
---

# Installing MongoDB

## Ubuntu 16.04

To install mongoDB on a Codeanywhere [container](http://docs.codeanywhere.com/connections/container.html) based on Ubuntu 16.04 distribution, just run the followings commands in your [terminal](http://docs.codeanywhere.com/overview/codeanywhereui/terminal.html) to install the latest official MongoDB release:

Import the public key used by the package management system.

 ```sh
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 9DA31620334BD75D9DCB49F368818C72E52529D4
```

Create a `/etc/apt/sources.list.d/mongodb-enterprise.list` file for MongoDB.
```sh
echo "deb [ arch=amd64,arm64,ppc64el,s390x ] http://repo.mongodb.com/apt/ubuntu xenial/mongodb-enterprise/4.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-enterprise.list
```

Reload local package database and install the MongoDB Enterprise packages.
```sh
sudo apt-get update
sudo apt-get install -y mongodb-enterprise
```

Start MongoDB
```sh
sudo systemctl mongod start
```

## CentOS 7.2
To install mongoDB on a Codeanywhere [container](http://docs.codeanywhere.com/connections/container.html) based on CentOS 7.2 distribution, just run the followings commands in your [terminal](http://docs.codeanywhere.com/overview/codeanywhereui/terminal.html) to install the latest official MongoDB release:

Configure repository with the `vim` editor:
```sh
sudo vim /etc/yum.repos.d/mongodb-enterprise.repo
```

Put the following contents in the file:
```sh
[mongodb-enterprise]
name=MongoDB Enterprise Repository
baseurl=https://repo.mongodb.com/yum/redhat/$releasever/mongodb-enterprise/4.0/$basearch/
gpgcheck=1
enabled=1
gpgkey=https://www.mongodb.org/static/pgp/server-4.0.asc
```

Install the MongoDB Enterprise packages
```sh
sudo yum install -y mongodb-enterprise
```

Start and enable MongoDB on startup
```sh
sudo systemctl start mongod
sudo systemctl enable mongod
```