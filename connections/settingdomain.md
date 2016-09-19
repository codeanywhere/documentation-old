---
current_menu: settingdomain
---

# Setting Custom Domain

Once you've created a container, you will probably want to preview it in your own link! Now, you can set your custom domain using our [Dashboard](https://codeanywhere.com/dashboard#)!

![customdomain1](images/customdomain1.png "customdomain1")

## CNAME Records
Before you start configuring your domain in Codeanywhere, there is one step you should do first and that is to go to your domain register (GoDaddy and similar) and create a CNAME record. 

The CNAME record you create must point to our proxy server: sfo.codeanyproxy.com

For more information on CNAMEs and how they work, please visit the Google Support Guide for CNAME records.

In your dashboard, select "Add New Domain Name".

## Add your Custom Domain:

Add External Port to 80, 443 or port in range of 1024 and 9999. Set the Internal Port to the port your application server is listening to. For example, if you set your Internal Port to 8000 and External Port to 80, you can access your custom domain without appending :8000 at the URL.

![customdomain1-1](images/customdomain1-1.png "customdomain1-1")

If you set the External port to 443, Codeanywhere will automatically set up a free SSL certificate provided by Let's Encrypt! It is important that you have already configured your CNAME record to point to Codeanywhere proxy server so the certificate can be issued.


![customdomain2](images/customdomain2.png "customdomain2")

Click on Create and that's it! Now you can access your Container from your domain!
Custom domains do not prevent container to be turned off in case it does not have AlwaysOn feature enabled.