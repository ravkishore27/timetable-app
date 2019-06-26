# timetable-app
An app for Timetable

#Install nodejs on AWS EC2 server:
The following procedure helps you install Node.js on an Amazon Linux instance.

To set up Node.js on your Linux instance
Connect to your Linux instance as ec2-user using SSH.

Install node version manager (nvm) by typing the following at the command line.

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
We will use nvm to install Node.js because nvm can install multiple versions of Node.js and allow you to switch between them.

Activate nvm by typing the following at the command line.
. ~/.nvm/nvm.sh
or
Just logout of the terminal and relogin, nvm will be loaded.

Use nvm to install the latest version of Node.js you intend to use by typing the following at the command line.
nvm install node
Installing Node.js also installs the Node Package Manager (npm) so you can install additional modules as needed.

Test that Node.js is installed and running correctly by typing the following at the command line.
node -e "console.log('Running Node.js ' + process.version)"
This should display the following message that confirms the installed version of Node.js running.
Running Node.js v4.4.5
