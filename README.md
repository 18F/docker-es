Docker ElasticSearch with NLP
=========
for the [Answers Platform](https://github.com/18f/answers)

Dependencies
---

[Vagrant](https://www.vagrantup.com/downloads.html) (>=1.6)

[Docker](https://docs.docker.com/installation/#installation)

- For OSX: I was successful with [boot2docker](https://github.com/boot2docker/osx-installer/releases). If you have issues with boot2docker or prefer a lightweight approach, try [this](http://zaiste.net/2014/02/lightweight_docker_experience_on_osx/).



To Get Started
---

1. Clone the repository `git clone git@github.com:18F/docker-es-nlp.git`
2. Tell Vagrant where to find Docker by setting `export DOCKER_HOST=tcp://localhost:2375`
3. Be sure docker is running (if using boot2docker run `boot2docker init` and `boot2docker up`) and pull down the trusted build from the docker registry with `docker pull dockerfile/elasticsearch`.
4. Fire up Vagrant with `vagrant up --provider=docker` from the project root.
5. Test elasticsearch with `curl -X GET 'http://localhost:9200/_status?pretty=true'`


Roadmap
---
- Add WordNet synonym library


Contributing
---

1. Fork it
2. Create your feature branch (`git checkout -b feature/my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
