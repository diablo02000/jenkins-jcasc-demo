# Docker Image

## Description

Create our Jenkins Docker image with all configurations and plugins than we need.
Our image will be based on [lts Jenkins Docker image](https://hub.docker.com/r/jenkins/jenkins).

## Install plugins

[Jenkins-plugin-cli](https://www.jenkins.io/doc/book/managing/plugins/#install-with-cli) is a cli tool to easelly install plugins without interaction in the web UI.
It takes a parameters a single plugin or a file with a plugins list to install.

- Create a txt file with a list of plugins to install:

```
blueocean:latest
job-dsl:latest
configuration-as-code:latest
git:latest
....
```

You can specify a version:

```
blueocean:1.43.0
```
