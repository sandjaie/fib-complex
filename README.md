[![Build Status](https://travis-ci.com/sandjaie/fib-complex.svg?branch=master)](https://travis-ci.com/sandjaie/fib-complex)

#### This project is a demo for multi container build and deploy

For Dev use Dockerfile.dev and docker-compose.<br>
>`$ docker build -f Dockerfile.dev .` <br>
> or `$ docker-compose up --build` <br>

For Prod use Dockerfile

Travis builds the image and pushes to docker hub. Ideally the below components should reside in their repos and have their own travis.yml to build, push and deploy.

* nginx
* server
* worker
* client