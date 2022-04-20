# Project 5

## Part 1: Docker Basics & Dockerfile

### Project Overview


### Run Project Locally

- How To Install Dockor and Dependencies 
   - `sudo apt install apt-transport-https ca-certificates curl software-properties-common` to install dependencies
   - WSL2 would not properly run Docker, so I installed Docker Desktop.
   
- How To Build a Container
   - Create `Dockerfile` in the project directory 
   - Once completed and inside project directory, `docker build .` builds the container
   
- How To Run the Container
   - `docker run -dit -p 8080:80 7caed60cb76d` where `7caed60cb76d` is the image ID

- How To View the Project
   - Open a browser and go to [localhost:8080](http://localhost:8080/)


## Part 2: GitHub Actions & DockerHub

### Create DockerHub Public Repo
1. On [DockerHub](https://hub.docker.com/), go to `Repositories`
2. Click the blue `Create Repository` button
3. Name the repo and add a description
4. Select `Public` for the repo visibility
5. Click the blue `Create` button at the bottom

### How to Authenticate with DockerHub via CLI using DockHub credentials
- Utilize the DockerHub Access Tokens
	- Under Profile, go to settings > Security > Access Tokens > New Access Token
	- Add a description, and select `Read, Write, Delete` for the Scope, then Click `Generate`
	- `docker login -u cybersmith22` entered into the command line will prompt for a password, enter the given token 

### Configuring GitHub Secrets 
- Needed the username and either a password or access token (recommended)
	- In the project GitHub repo, go to Settings Tab > Secrets > Actions > New repository secret
	- Give the secret a name and value, then click `Add Secret`

### Behavior of GitHub workflow
what does it do and when
variables to change (repository, etc.)


## Part 3: Deployment
### Container Restart Script
what it does


### Webhook Task Definition File
what it does


### Setting Up a Webhook on the Server
How you created you own listener
How you installed and are running the webhook on GitHub

### Setting Up a Notifier in GitHub or DockerHub




## Part 4: Diagramming 

### Integration Workflow Diagram

### Deployment Workflow Diagram


## Resources

[GitHub Discord Action](https://github.com/marketplace/actions/discord-action)
