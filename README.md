# SmartBoxDocker

... provides a complete setup for the SmartBox App including the required backends as well as the Web Application as Docker containers. 
... added Homebridge Gateway

## Installation
SmartBoxDocker requires [Docker](https://www.docker.com/) .
  - Download this app repository
```sh
$ git clone https://github.com/rockydaddy/SmartBoxDocker.git
```
  - Update the Sonos and the RC433 configuration an to point to the API Server addresses (use a text editor of your choice, here it's vi)
```sh
$ vi ./smartboxapp/data/config.js
```
  - update `var basisUrl = "http://192.168.0.6:5005/";` pointing to your Sonos and the RC433 backend API servers
  - start composing and running the docker containers
```sh
$ docker-compose up -d
```
- Please see README.md on https://github.com/rockydaddy/SmartBoxApp.git for further description of the App
