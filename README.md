# Orchestration

This repo holds orchestration logic on how to spin up the infrastructure.

## Local Environment

This will spin up everything locally!!

## Set Up

### Docker

We recommend installing [Docker Desktop](https://www.docker.com/get-started "Docker Desktop Get Started") as it includes compose and other Docker apps.
Documentation: [Docker docs](https://docs.docker.com/compose/install/ "Docker Desktop Get Started")

### Development WorkFlow

The application is composed of [Frontend](https://github.com/robinferm/jobs-in-sweden-FE "Frontend Repo") and [Backend](https://github.com/robinferm/jobs-in-sweden-BE "Backend repo") services. For orchestration to work properly all three repositories should be cloned in the same containing folder:

```
FOLDER
├── backend
├── frontend
└── Compose
```

Run docker images in detached mode & print new containers.

```
cd Compose Folder

docker-compose -p JIS -f docker-compose.yml -f docker-compose-dev.yml up -d --build
```
