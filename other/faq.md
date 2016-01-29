---
current_menu: otherq
---

# FAQ

> Why is working with FTP slower on Codeanywhere then with the FileZilla?

While working with FileZilla you are directly connected from local computer to your server, on the other hand the Codeanywhere is acting as a "middle man" between user and ftp - any action done by user is firstly processed at our server and then sent to the ftp. Same thing works in opposite direction, ftp sends response to Codeanywhere and then Codeanywhere forwards the response back to user.
Also, the speed of the server response is depending on the server location. If your server is located it America, the response will be faster, but if it's located in China it will be slower. 
We do however plan to expand our server coverage around the world for faster connections.


> How can I connect to Local FTP/SFTP Server?

Codeanywhere uses its file services in the cloud that are used for making connections.
Behind the scenes it looks something like this: 

Codeanywhere Web or mobile app---->Codeanywhere API---->Codeanywhere File Service---->Your FTP/SFTP Server

Your FTP/SFTP server is in your local network and the only way you could connect to your server from Codeanywhere is that you use port forwarding on your router to your local FTP/SFTP server. The other problem that could come in your case is your router's public IP. If your internet provider does not provide you a static IP, then you would also need to use some of DDNS services.



> Why is my server not responding after I made few requests, but after an hour works fine again?

While performing actions using Codeanywhere, the requests are sent from our app to your server. Sometimes the number of requests are causing your server to block the requests and add Codeanywhere to the blacklist. To avoid this you must make sure that your server is reachable from the following IP addresses:

 - 54.69.152.243
 - 54.186.244.104
 - 54.187.136.143
 - 54.187.142.118
 - 54.187.182.165
 - 54.187.44.75
 - 54.191.40.18

If you have no administration rights on the server, please ask your administrator whitelists these IP’s. 



> I can't see organizations repositories. How can I setup this?

You have to explicitly allow Codeanywhere to access your organizations. You can do it in two ways:

1.) During authorization process
Click Grant / Request Access on organization which repositories you want to access through Codeanywhere

<img src="images/pic1.png" width="300" height="auto">

2.) While logged in your GitHub account, click Account -> Settings -> Applications -> Codeanywhere
Click Grant / Request Access on organization which repositories you want to access through Codeanywhere

<img src="images/pic2.png" width="300" height="auto">

After allowing organization access, you can list your repositories through Codeanywhere.

> Is it possible to deploy to Heroku?

Deploying with Heroku requires you to install Heroku toolbelt. You can install it using SSH command:

```sh	
	wget -O- https://toolbelt.heroku.com/install-ubuntu.sh | sh
```

Now you can use Heroku CLI. More detailed instruction can be found on official Heroku toolbelt website https://toolbelt.heroku.com/




> Why doesn't my Ruby stack work?

Please change IP address on your container from 127.0.0.1 to 0.0.0.0 so that you could be able to preview your Ruby box. You can do that inside Config - under commands - of your container (right click on your container and select Config). 
You just have to use the following command in order to run your Rails container: "rails s --binding=0.0.0.0" 
This will override localhost (127.0.0.1) where your app can't work.	



> In a Wordpress stack, after uploading plug-ins, I receive an error and permission is denied. Why?

You can prevent these issues by running commands in SSH: 
- Ubuntu: 
```sh
	sudo chown cabox:www-data -R ~/workspace 
```
- CentOS: 
```sh
	sudo chown cabox:apache -R ~/workspace
```

Also, please download original plug-ins from Wordpress, so you don't receive this error again. 


> I receive the following error when trying to access Google Drive: Invalid token. What could cause this?

There seems to be something wrong with your long-term access token, so please try removing and adding your Drive account. If that does not work please try revoking access to Codeanywhere from your Google security page located at: [https://www.google.com/settings/security](https://www.google.com/settings/security) and afterwards try to add it again.

<img src="images/google-invalidtoken.png" width="500" height="auto">

> How to connect container to Putty?

Here are the complete instructions for connecting your container to Putty:

To generate a set of RSA keys with PuTTYgen: 
	1. Start the PuTTYgen utility, by double-clicking on its .exe file
	2. For Type of key to generate, select SSH-2 RSA
	3. In the Number of bits in a generated key field, specify either 2048 or 4096 (increasing the bits makes it harder to crack the key by brute-force methods)
	4. Click the Generate button 
	5. Move your mouse pointer around in the blank area of the Key section, below the progress bar (to generate some randomness) until the progress bar is full
	6. A private/ public key pair has now been generated
	7. In the Key comment field, enter any comment you'd like, to help you identify this key pair, later (e.g. your e-mail address; home; office; etc.) -- the key comment is particularly useful in the event you end up creating more than one key pair
	8. Click the Save public key button & choose whatever filename you'd like (some users create a folder in their computer named my_keys)
	9. Click the Save private key button & choose whatever filename you'd like (you can save it in the same location as the public key, but it should be a location that only you can access and that you will NOT lose! If you lose your keys and have disabled username/password logins, you will no longer be able log in!)
	10. Right-click in the text field labeled Public key for pasting into OpenSSH authorized_keys file and choose Select All
	11. Right-click again in the same text field and choose Copy.

Container config: 
	1. Log on to your container 
	2. Run: vim ~/.ssh/authorized_keys 
	3. Paste key in new line 
	4. Save and exit

Putty config: 
	1. Start PuTTY by double-clicking its executable file; 
	2. PuTTY's initial window is the Session Category (navigate PuTTY's various categories, along the left-hand side of the window); 
	3. In the Host Name field, enter the Container’s DNS 
	4. Enter the port number in the Port field (see Container info) 
	5. Select SSH under Protocol; 
	6. Along the left-hand side of the window, select the Data sub-category, under Connection; 
	7. Specify the username cabox in the Auto-login username field; 
	8. Expand the SSH sub-category, under Connection; 
	9. Highlight the Auth sub-category and click the Browse button, on the right-hand side of the PuTTY window; 
	10. Browse your file system and select your previously-created private key; 
	11. Return to the Session Category and enter a name for this profile in the Saved Sessions field 
	12. Click the Save button for the Load, Save or Delete a stored session area.

> How can I connect to a Container via FTP?

You can't connect via FTP but you can connect as SFTP. These are the credentials you'll need: 
Hostname: preview link of your container - looks something like preview.xxxx.box.codeanywhere.com and you can check it in Container's Info with a right click on your Container 
User name: cabox 
As for the password, you can't connect this way. You'll need private key of your Container and you can get it by going to /home/cabox/.ssh/id_rsa and that's your private key which you can use for connecting to your Container. 
Also, you'll need to check your Port - right click on your Container, select Info, locate SSH Terminal listening on port, and that's the port you have to use for connecting to SFTP.

> How can I find private and public key of my Container?

You can view Private Key of your container by going to cd /home/cabox/.ssh/ using your SSH terminal. There you will find: 
- id_rsa - private key container of your container, 
- id_rsa.pub - public key of your container.


> How can I connect to the MySQL Database on my container?

Download your private key from Codeanywhere editor to your local machine and change the file permissions (for Mac and Linux):
```sh
	$chmod 600 codeanywhere.pem
```
Get the SSH port and DNS of your Container from the Info - accessible with a right click on your Container. Create a tunnel from your local machine to your Container (via terminal):

```sh	
   $ssh -L 3306:localhost:3306 cabox@ssh.{CONTAINER-DNS} -p {CONTAINER-SSH-PORT} -i codeanywhere.pem
```

Now you can connect to your remote MySQL using: localhost:3306

![sshconnection](images/sshconnection.png "sshconnection")


> How can I change Preferences? All I get is a JSON file.

In our current version, it is possible to override settings from Preferences -> Default, inside Preferences -> User/Project.

For example, in Preferences -> Default -> General, you'll see it is set to: 
```
"workspace": { 
	"theme": "monokai" 
} 
```
And now you can change it inside Preferences -> User/Project -> General, by adding code:
```
"workspace": { 
	"theme": "white" 
}
```
And by doing this, you'll override settings from Default. We'll keep updating this so stick around!

> How can I connect to Bitbucket via authorized_keys

The recommended method is adding Codeanywhere SSH key to your Bitbucket account. That way, you can push commits to your private repo without password prompt. To do so, copy your Codeanywhere public key (you can find it by clicking your email in editor, then click "get your public key") and paste it to your bitbucket account (Account -> manage account -> SSH keys -> add Key)

Now your Codeanywhere account is authorized to make changes to your repo.

If you already have repository in Bitbucket, just by cloning your repository, your git will be setup. If you have existing project with empty Bitbucket git repository, you can add your repo with "git remote add origin {GIT_SSH_URL}". You can find your {GIT_SSH_URL} by clicking clone in bitbucket repo, then copying url next to 'git clone', its format is git@bitbucket.org:/username/repository.git

now you have successfully setup your git. 


> How can I work with my repository with Codeanywhere

Connect to your repository via [Github](http://docs.codeanywhere.com/connections/github.html) or [Bitbucket](http://docs.codeanywhere.com/connections/bitbucket.html) directly or with [Git From URL](http://docs.codeanywhere.com/connections/gitfromurl.html). You can push changes to your repository using standard git commands inside your SSH terminal:

git add -A // To track all files

git commit -am "message" // To commit changes

git push origin master // Push your local changes to repository

