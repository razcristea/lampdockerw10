---
platforms: Windows 10
Author: Dan Patrascu-Baba
---
# Building a LAMP development eviroment on Windows 10 using Docker

This sampel shows how PHP developers working on Windows 10 clients can set up a full LAMP development environment within few secons using Docker for Windows. This will allow you to create two containers, one running a Linux VM with Apache installed and one running the MySQL database. After you have completed all steps and go to a broser and navigate to localhost:8080 you will be able to see the phpinfo page.  

## Prerequsites
To create a LAMP development environment on Windows 10 using Docker for Windows, you will need: 
1. Docker for Windows
2. A code editor that includes a terminal (I used Visual Studio Code)

## Steps
### 1. Install Docker for Windows

You can dowload and install Docker for Windows from the official [Docker] (https://docs.docker.com/docker-for-windows/install/#download-docker-for-windows). If you follow the installation guide on the same page, all necessary components will be installed, including `docker-compose`, which is a vital component. 

Also make sure that the C drive is shared with Docker. You can do this by right clicking the Docker icon, Settings and shared drives.

### 2. Clone or Download repostiory
This is a very simple sample so you can simply recreate the files if you are not familiar with Github or you cand download or clone [the repository](https://github.com/danpdc/lampdockerw10)

Alternatively, from your shell or command line, use:

`git clone https://github.com/danpdc/lampdockerw10.git`

### 3. Run docker-compose
On your code editor you need to bring up the terminal window (if it's not already there) and run the following command to build the environment:

'docker-compose up'
### 4. Check your environment
If everything is configrued correctly, you should be able to open a browser, navigate to localhost:8080 and see the phpinfo page. This means that your development environment is up and running and you can start coding. 

### 5. Stop docker containers
In order to stop the docker containers created previously, you can open up your terminal window and run the following command: 
'docker-compose stop'

This will stop your web server and MySQL instance. 

Hope this will save you the time I needed as a php and Docker rookie to get this up and running. 
