# Introduction
Docker In Docker (also known as dind) allows developers to run a [Docker](https://blog.packagecloud.io/what-is-docker-a-beginners-guide/) container within an already running Docker container to support CI/CD pipelines and create sandboxed container environments. 

# Why Would You Run Docker In Docker?
Running Docker in Docker gives developers more flexibility to take advantage of the tool to accomplish tasks that might be more difficult to accomplish via other means.

# The benefit of Docker in Docker
The first is to run CI systems such as GitLab or Jenkins on-premises on Docker containers. In this case, you can run Docker containers for each programming language/dependent middleware in the container and then create Docker images for production use, etc. This has the advantage of nested usage of Docker.

Docker as a sandbox environment. Suppose you want to use a Docker container as an environment isolated from the host environment where the actual work is done. In that case, you can launch a Docker container within that container. Building a sandbox environment inside a container is very easy because the environment can be disposed of by simply destroying the container.

# Docker in Docker by using Sysbox 
Sysbox is an open-source dedicated container runtime that can nest containers without requiring privileged mode

## Benefits
- Preload Container Images
- Hardened Security
- Containerized Dev Environments

 

