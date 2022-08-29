# Django REST Framework and Docker

## A Beginner's Guide To Docker

### Docker Definition

Docker is way to isolate and run entire applications such that virtual environments aren't needed. It does this largely through the process of virtualization through cotainerization.

### Images and Containers

Image: In docker, an image refers to a snapshot in time of what a project contains

Container: A container is a running instance of a Docker image

Each image is built of either one or more image layers. Each image layer is an immutable unchanged thing like a git commit, so that there is no discrepancy between two devs working on the same project. The changes are also cached in the project as the project is built, which eventually helps with the performance of the app as a whole.

Once created and wired up correctly, a Dockerfile can completely replace a virtual environment in a Django project.

## Django REST Libraries

As far as I can tell this reading was all about how to setup a basic Django site, a process that we spent the last week covering.

## Things I want to know more about

* Docker is still pretty nebulous to me in terms of what it actually is and how it runs. I think I will need to see it in action to understand it on more of a conceptual level.
