# timetable-app
An app for Timetable
```
git clone <link>
cd timetable-app
npm install
npm start &\
or\
npm run build &
```

# Install nodejs on AWS EC2 server:
The following procedure helps you install Node.js on an Amazon Linux instance.

To set up Node.js on your Linux instance
Connect to your Linux instance as ec2-user using SSH.

Install node version manager (nvm) by typing the following at the command line.

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
We will use nvm to install Node.js because nvm can install multiple versions of Node.js and allow you to switch between them.

Activate nvm by typing the following at the command line.
. ~/.nvm/nvm.sh or\
sudo bash nvm.sh\
or
Just logout of the terminal and relogin, nvm will be loaded.

Use nvm to install the latest version of Node.js you intend to use by typing the following at the command line.
nvm install node\
or
nvm install 10.16.0\
Installing Node.js also installs the Node Package Manager (npm) so you can install additional modules as needed.

Test that Node.js is installed and running correctly by typing the following at the command line.
node -e "console.log('Running Node.js ' + process.version)"
This should display the following message that confirms the installed version of Node.js running.
Running Node.js v4.4.5

# Install npx
sudo npm install npx

# Create timetable-app
npx create-react-app timetable-app\
cd timetable-app\
npm start

# Install Git
sudo yum install git

# Configure git repository on your AWS machine
Setup ssh keys in your local machine. Import the public key to Git setting > SSH keys.\
git config --global user.email "username@gmail.com"\
git config --global user.name "name"\
git init      (in the app folder)\
git remote add origin git@github.com:ravkishore27/timetable-app.git\
git pull origin master\
git add .\
git commit -m "message"\
git push origin master\
git clone <current repository> (if required).


# AWS Amplify
- Login into AWS console.
- Navigate to AWS Amplify
- Deploy the timetable-app using github as Repository Service.
- Remember that github (remote) app when updated with commits, Amplify will build, deploy and verify.


