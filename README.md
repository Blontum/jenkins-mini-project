# Jenkins Installation and Setup

## Table of Contents
1. [Install Java](#install-java)
2. [Add Jenkins to the Debian Repository](#add-jenkins-to-the-debian-repository)
3. [Install Jenkins](#install-jenkins)
4. [Enable Port 8080 on the Host Firewall](#enable-port-8080-on-the-host-firewall)
5. [Install Docker on the Ubuntu Local Server](#install-docker-on-the-ubuntu-local-server)
6. [Setup Git Plugin on Jenkins](#setup-git-plugin-on-jenkins)
7. [Install Docker Publish Plugin](#install-docker-publish-plugin)

## Install Java
1. Run `sudo apt update -y`
2. Run `sudo apt install openjdk-8-jdk`

## Add Jenkins to the Debian Repository
1. Run the provided wget and apt-key add commands to add the Jenkins repository.

## Install Jenkins
1. Run `sudo apt update`
2. Run `sudo apt install Jenkins`
3. Run `sudo systemctl start jenkins`

## Enable Port 8080 on the Host Firewall
1. Run `sudo ufw enable`
2. Run `sudo ufw allow 8080`
3. Run `sudo ufw allow OpenSSH`

## Install Docker on the Ubuntu Local Server
1. Follow the official Docker documentation.
2. Run `sudo usermod -a -G docker jenkins`
3. Run `sudo systemctl restart jenkins`

## Setup Git Plugin on Jenkins
1. Add the public GitHub repository location.
2. Set up the branch to pull from.

## Install Docker Publish Plugin
1. Set up the Docker plugin.
2. Enter the repository and image name to publish.

Please follow the steps above to install and set up Jenkins with the necessary plugins and configurations to enable a Docker-based pipeline.