# Dokku Monitoring, based on node_exporte, cAdvisor, prometheus and grafana.

-----------------------------------------
#docker compose commands to be implemented.
`docker-compose up -d`
`docker-compose stop`
...

# dock
`docker run \
-v $(pwd)/docker-compose.yml:/docker-compose.yml \
-v $(pwd)/.env:/.env \
-v $(pwd)/config:/config \
-v /var/run/docker.sock:/var/run/docker.sock \
docker/compose:1.23.2 up -d`


`docker run \
-v $(pwd)/docker-compose.yml:/docker-compose.yml \
-v $(pwd)/.env:/.env \
-v $(pwd)/config:/config \
-v /var/run/docker.sock:/var/run/docker.sock \
docker/compose:1.23.2 <command>`
