# Wordpress Demo

## Running on Docker
The project can be run locally using Docker and Docker Compose.

The following instructions provide details on how to deploy the project using Docker Compose.  This method of deployment is intended for local development and demonstration purposes.  It is **NOT** intended to support production level deployments where security, availability, resilience, and data integrity are important.


## Benefits

The benefits to using this approach are;
* Ease of getting the project up and running on your local system.
* Builds the images using the source code from your local working copy.

## Prerequisites

* Docker and Docker Compose
  * Install and configure Docker and Docker Compose on your system.  The recommended approach is to use either [Homebrew](https://brew.sh/) (MAC) or [Chocolatey](https://chocolatey.org/) (Windows) to install Docker (which includes Docker Compose).
* If you are working on Windows, use Git Bash (or equivalent shell) to run the scripts.
* Fork and clone a local working copy of the project source code.
* Open a command/shell window to the project's `./wp-content` folder.

## Building the Images

The first thing you'll need to do is build the Docker images.  

To build the images run:
```
docker build -t 'wp-image' .
```

## Starting the Project

To start the project run:
```
docker-compose up
```

This will start the project interactively; with all of the logs being written to the command line.  Press `Ctrl-C` to shut down the services from the same shell window.


## Using the Application

* The UI is exposed at; http://localhost:8000/
