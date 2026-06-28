# Node.js Application Deployment on Amazon Linux (EC2)
## Introduction
This is my another project where I deployed a Node.js application on an Amazon Linux EC2 server.
In this project, I learned how Node.js works as its own server, so no external web server like NGINX or Apache is required. The application files (app.js and package.json) were provided by my mentor through a GitHub URL, and I deployed the project by cloning and running it on the server
## Architecture
![alt text](<imgs/nodejs architecture.jpeg>)

## Technologies Used
* Amazon Linux (EC2)<br>
* Node.js<br>
* NPM (Node Package Manager)<br>
* Git<br>
## Features
* Node.js runs its own server
* No need for NGINX or Apache
* Application runs using node app.js
* Accessible via EC2 public IP and port
## Setup & Deployment Steps
### 1.Launch EC2 instance
* Create Amazon linux EC2 instance 
![alt text](<imgs/creating ec2 instance.png>)
* Connect using SSH
![alt text](<imgs/connect ec2 throgh ssh.png>)
### 2.Install Git
sudo yum update <br>
sudo yum install git -y
![alt text](<imgs/install nodejs and git.png>)
### 3.Clone Project from Github 
git clone <my url here >
![alt text](<imgs/clone project from github.png>)
### 4.Go Inside Project Folder
cd nodejs.app
![alt text](<imgs/go inside project folder.png>)
### 5.Install Dependencies
npm install
![alt text](<imgs/installing dependencies.png>)
### 6.Run Application 
node app.js
![alt text](<imgs/run application.png>)
### 7.Access Application
* open browser
* Enter->
your-ec2-public-ip:port
* Application Will be Live 
![alt text](<imgs/access website 2.png>)
## What I Learned
* Basics of Node.js
* Running server using Node.js
* Using npm to install dependencies
* Deploying application on EC2
* Difference between Node.js and NGINX/Apache
## Future Improvements
* Use PM2 to keep app running
* Add domain name
* Enable HTTPS
* Deploy using Docker
## Summery
This project helped me understand how
Node.js works as a server and how to 
deploy applications without using  
traditional web servers.
It is an important step in learning backend development, DevOps, and cloud deployment.