# puppetstack
Running puppet stack on windows as a linux container

## Setup
```
docker volume create --name puppetdb-postgres-volume -d local
docker-compose up
```

## Troubleshooting

At first try the containers failed to start up for me with port related errors.

* Ensure that no other programs are using the ports mapped in the docker-compose.yaml file
* I had to install the latest docker experimental on windows 10 to be able to start (2.0.4.1 edge channel) otherwise kept getting startup failures.
