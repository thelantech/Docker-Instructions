# Docker-Instructions
Instructions for implementing Docker Cloud into the Github workflow
<br><br><br>
<img src="https://upload.wikimedia.org/wikipedia/commons/7/79/Docker_%28container_engine%29_logo.png">
<br><br>
<h2>Overview</h2>
Docker is a container service which ensures that there are no dependency or configuration gaps between development environments and other environements or servers. It can be integrated directly into a Github version control workflow and makes up an essential part of a continuous integration development cycle. 

At its core, docker uses something called a 'Dockerfile' to configure the building of a container which sets up the necessary environment for the app which is being developed. This is included with the source code and ensures that every time someone implements the source code, all they have to do is build the Dockerfile and they will have an identical environment in which to run the app. 

<h2>Getting Started</h2>

<h3>Installation</h3>

Firstly, Docker needs to be installed on your system. Refer to the documentation <a href="https://www.docker.com/community-
edition"> here</a> for instructions on how to install and begin using docker. Docker has a very well-maintained set of docs and 
video tutorials, so I would highly reccommend acquainting yourself with the basics of Docker usage through these. A good place to start is the Docker tutorial <a href="https://docs.docker.com/get-started/#setup">here</a>.  

<h3>Configuration</h3>

For continuous integration, you will need to sign up for a <a href="https://cloud.docker.com/">Docker CLoud</a> account. Once you have signed up

<h3>Workflow</h3>

Once you have acquainted yourself with the basics of Docker usage, it is time to implement it into your workflow. There are two 
ways in which you will be working with Dockerfiles and containers, <b>Creating</b> new projects, and <b>Pulling</b> existing 
ones from the <b>Docker Cloud</b>.

<h3>Creating a New Project</h3>

The point of <b>Docker</b> is to create self-contained environements for each app or service that you are working on. This means that you don't have one development environment, so much as one <i>for each project</i>. 

With that in mind, the workflow for creating a new project is as described in the tutorial linked above. 
1. Create a new directory and a short script to test the environment
2. Create a requirements.txt
3. Create a Dockerfile
4. run 'docker build -t (your_tag_here) ." *Note the punctiation mark at the end. This will tell Docker to use the local Dockerfile.




