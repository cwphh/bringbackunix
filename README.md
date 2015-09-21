#bringbackunix.com

Set up a working, publically accessible full stack MEAN Application on a Digital Ocean Droplet with this tutorial.

###1. Set up and configure Digital Ocean Droplet

IP Address of our droplet is: 46.101.49.106

1. Create a new MEAN droplet
2. Login as root and configure a new user
3. Configure firewalls and SSH security

https://www.digitalocean.com/community/tutorial_series/new-ubuntu-14-04-server-checklist

at the end of this process we will be able to login via terminal using this command

```ssh -p 1968 listingslab@46.101.49.106```

###2. Add Project to to Github and deploy it to the droplet

https://developer.github.com/guides/delivering-deployments/

SSH Deploy keys
https://help.github.com/articles/generating-ssh-keys/
on server

```ssh-keygen -t rsa -b 4096 -C "listingslab@gmail.com"```

```cat ~/.ssh/id_rsa.pub```

###3. Install Express with the Express application generator

http://expressjs.com/starter/generator.html

```listingslab$ express bringbackunix --git -c less --ejs ```