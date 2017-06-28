# Run Node and Chrome Headless in a container

This repo contains the Dockerfile for running Node 6 and Headless Chrome in a docker container. It is designed to mount the test application as a volume and run the test command for your project.

Replace `npm test` with whatever command is used to run your tests.

```
docker run -i --privileged -v `pwd`:`pwd` -w `pwd` gnomeontherun/docker-node-chrome-headless npm test
```