Dependencies
-----

Vagrant (>=1.6) - https://www.vagrantup.com/downloads.html

Docker - https://docs.docker.com/installation/#installation
OSX: I was successful with [boot2docker](https://github.com/boot2docker/osx-installer/releases)
If you have issues with boot2docker or prefer a lightweight approach, try http://zaiste.net/2014/02/lightweight_docker_experience_on_osx/

VirtualBox - https://www.virtualbox.org/wiki/Downloads


To Get Started
-----

1. Clone the repository `git clone git@github.com/alskdjfaksdjf.git`
2. Be sure docker is running (if using boot2docker run `boot2docker init`) and pull down the trusted build from the docker registry with `docker pull dockerfile/elasticsearch`.
3. Fire up Vagrant with `vagrant up --provider=docker`.
4. Test elasticsearch with `curl -X GET 'http://localhost:9200/_status?pretty=true'`