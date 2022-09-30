# Synapse-deployment

This is a docker deployment of Matrix Synapse. Using this project you can deploy a single instance of Synapse on a machine.
This repo contains yaml files,plain text config files, json files and pem files which are needed for deployment.

You should change the variables and names to make use of it.

The file structure is as follows:

1- **certificates**: Contains TLS certificates.

2- **element-web**: Contains frontend and nginx webserver configs.

3- **synapse**: Contains Matrix Synapse homeserver config file.

4- **.env.example**: Consists of environment variables to be used for database, etc.

5- **docker-compose.yml**: Main docker compose file to deploy our services.

## Deployment
To deploy Synapse first change the .env.example to .env:
```
mv .env.example .env
```
Then run the services
```bash
docker-compose up -d
```