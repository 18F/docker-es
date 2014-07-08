Docker ElasticSearch with NLP
=========
for the [Answers Platform](https://github.com/18f/answers)

Dependencies
---

[Vagrant](https://www.vagrantup.com/downloads.html_ (>=1.6)

[Docker](https://docs.docker.com/installation/#installation)

- For OSX: I was successful with [boot2docker](https://github.com/boot2docker/osx-installer/releases). If you have issues with boot2docker or prefer a lightweight approach, try [this approach](http://zaiste.net/2014/02/lightweight_docker_experience_on_osx/).



To Get Started
---

1. Clone the repository `git clone git@github.com:18F/docker-es-nlp.git`
2. Be sure docker is running (if using boot2docker run `boot2docker init`) and pull down the trusted build from the docker registry with `docker pull dockerfile/elasticsearch`.
3. Fire up Vagrant with `vagrant up --provider=docker` from the project root.
4. Test elasticsearch with `curl -X GET 'http://localhost:9200/_status?pretty=true'`