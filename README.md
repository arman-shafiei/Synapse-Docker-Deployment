# Synapse-deployment

This is a docker deployment of Matrix Synapse. Using this project you can deploy a single instance of Synapse on a machine.
This repo contains yaml files,plain text config files, json files and pem files which are needed for deployment.

You should change the variables and names to make use of it.

The file structure is as follows:

- **certificates**: Contains TLS certificates.

- **element-web**: Contains frontend and nginx webserver configs.

- **synapse**: Contains Matrix Synapse homeserver config file.

- **.env.example**: Consists of environment variables to be used for database, etc.

- **docker-compose.yml**: Main docker compose file to deploy our services.

## Deployment
To deploy Synapse first change the .env.example to .env:
```
mv .env.example .env
```
Then run the services
```bash
docker-compose up -d
```
