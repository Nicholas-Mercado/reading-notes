# Django REST Framework & Docker

## Beginner’s Guide to Docker

**Docker** - is a tool used to automate the development of apps in a container so apps can work in different environments

The docker container holds all the dependencies for a application. This allows for:

- multiple containers to run on the same hardware
- each container are in isolated environments
- high productivity
- fast to configure

### Image and Containers

**Image** - a snapshot in time of a project

**Container** - a running instance of the image

#### Creating a custom image terminology

- Dockerfile is the instructions for a image
- image is a snapshot of the instructions at a specific time
- docker-compose.yml says how to make the image

### Create a image

First create a local directory and inside place a python folder

```python
cd ~/Desktop
$ mkdir code && cd code
$ mkdir python3.7 && cd python3.7
```

Create a Dockerfile

```python
touch Dockerfile
# in Dockerfile add this code
FROM python:3.7-alpine
```

### Build Images

```python
# Don’t forget that period . at the end of the command!
docker image build .
```

Use  to check

```py
docker image ls
```

[A Beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

[Django for APIs](https://djangoforapis.com/library-website-and-api/)

[What Is Docker?](https://www.youtube.com/watch?v=rOTqprHv1YE)
