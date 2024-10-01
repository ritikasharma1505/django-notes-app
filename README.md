# Simple Django CI/CD Project 
This is a simple notes app built with React and Django.
This repo is not cloned locally..only remotely this project is available


## Requirements
1. Python 3.9
2. Node.js
3. React

## Installation
1. Clone the repository
```
git clone https://github.com/LondheShubham153/django-notes-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the app
```
docker run -d -p 8000:8000 notes-app:latest
```

## NOTE : Nginx

Install Nginx reverse proxy to make this application available

`sudo apt-get update`
`sudo apt install nginx`


Troubleshooting steps :
This was hard until GitHub hooks came into the picture, make sure the same git repo is used in Jenkinsfile for which you created GitHub webhooks(which means fork the project), I mistakenly used the instructor's, and the auto build trigger wasn't working

