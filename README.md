# Web implementation of PythonBuddy + Sandbox

Uses [Docker Python Sandbox](https://github.com/christophetd/docker-python-sandbox) library to Sandbox [PythonBuddy](https://github.com/ethanchewy/PythonBuddy).

Created off of [christophetd/code-execution-api-demo](https://github.com/christophetd/code-execution-api-demo)

### Prerequisite:
* Install Docker and Node.js
* Running on Linux Server

### System requirements:
* 4GB of Storage
* 1GB of RAM

### Steps:

#### 1. Clone PythonBuddySandbox
    `git clone https://github.com/ethanchewy/PythonBuddySandbox`
    
#### 2. Clone PythonBuddySandboxed
    `git clone https://github.com/ethanchewy/PythonBuddySandboxed`
    
#### 3. CD into the folder
    `cd PythonBuddySandbox/container`
    
#### 4. Build an image of the docker-sandbox
    `docker build -t christophetd/docker-sandbox .`
    
#### 5. Come back to the home location
    `cd`

#### 6. Install docker-python-sandbox-pythonbuddy
    `npm install --save docker-python-sandbox-pythonbuddy`
    
#### 7. CD into the PythonBuddySandboxed
    `cd PythonBuddySandboxed`
    
#### 8. Copy config details to a Config.js
    `cp api/config.js.sample api/config.js`

#### 9. Start
    `sudo npm start`

#### *Remember!! Change `config.js`'s `config.security.secret`to something different and change static/js/javascript.js in PythonBuddySandboxed to the same secret!!*

Navigate to `localhost:3000 `to see PythonBuddy Dockerized!

(Or if you are hosting, navigate to `ExternalIP:3000 `to see PythonBuddy Dockerized!)

More documentation coming...   
