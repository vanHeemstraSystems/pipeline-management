pipeline-management
# Pipeline Management

A template for a microservice.

Can be read as "Pipeline Management" at https://app.gitbook.com/???/????/

Can be browsed as "Pipeline Management" at https://vanheemstrasystems.github.io/pipeline-management/

Documentation of this repository is automatically done with Quarto using GitHub Actions

Based on "n8n" at https://n8n.io/

Based on "n8n Docker Deployment" at https://docs.n8n.io/hosting/installation/docker/

Based on "n8n on Docker Hub" at https://hub.docker.com/r/n8nio/n8n#start-n8n-in-docker

Based on "NGinX Proxy Manager" at https://nginxproxymanager.com/

Based on "Awesome Quarto" at https://github.com/mcanouil/awesome-quarto

Based on "Quarto Web" at https://github.com/quarto-dev/quarto-web and https://quarto.org/

Based on "Creating your personal website using Quarto" at https://ucsb-meds.github.io/creating-quarto-websites/

Create yarn.lock file as follows:

```
$ cd containers/app/main
$ yarn install
```

Run as follows:

```
$ cd containers/app
$ docker-compose --file docker-compose.dev.yml --project-name pipeline-management-dev up --build -d
```
