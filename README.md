# termux-nodejs-test

Wget https://github.com/hakamimmmm/termux-nodejs-test



This sounds surprising but yet it is possible,I was fascinated by the idea that with out deploying my node app ,i can make it mobile(ready to use any where).So I am going to make a node app with a simple get method and run it in android termux and broadcast it using localhost.run
First thing we need to install Termux in our android phone ,it is available in Playstore.
After installing Termux ,give the permission to storage in app settings(important).
Then we need to update and upgrade termux from its terminal.
Open termux and type in the below commands
apt-get update && apt-get upgrade
After it is done, we need to install node js ,ssh and git for server ,broadcast and code update respectively.
node js
apt install nodejs
ssh
apt-get install openssh
git
pkg install git
That’s it !!that’s all we need!!
Now, clone this repo in your termux ,navigate into it and install the packages and start the server
npm install && node server.js


Now open a new session in termux and type in
ssh -R 80:localhost:3000 ssh.localhost.run
It will generate two links(http and https),just copy the links and use it any where,any system.You can see the response sent by your node server running in android mobile.Which is cool!!!!
cons
