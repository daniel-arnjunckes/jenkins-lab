# Jenkins Lab

## Introduction

A jenkins lab environment to test/learn about this application. 

## Architecture

Run the docker compose file to build the environment, this will set to you on your docker the following components:
- 1 Jenkins container, with a ssh-key pair to use
- 1 Docker DinD(Docker in Docker), so you can have some fun with Jenkins' Docker plugin, using dymanic agents
- 1 Jenkins Docker Agent(ssh-agent image), so you can try and create a manual agent to run your jobs

When done, this is what you will have running on your docker:
![Architecture](./imgs/lab_architecture.png)

> Important note: In this lab, you will have a DinD container with TLS deactivated, don't try this in production envs