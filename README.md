# docker-nodejs-wikidata
Docker image with convenient NodeJS wikidata tools

Building the image:

    docker build -t nodejs-wikidata .

Image can also be found at: https://hub.docker.com/r/toniher/nodejs-wikidata/

Executing Docker image (we mount /scripts, accessible then from host)

    docker run -d -v $PWD/scripts:/scripts  --name nodejs-wikidata nodejs-wikidata tail -f /dev/null

    docker exec -ti nodejs-wikidata /bin/bash


