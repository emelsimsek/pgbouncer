 docker-compose -f .containers/docker-compose.yml build  --build-arg SSH_KEY="$(cat ~/.ssh/id_rsa)"

 docker-compose -f .containers/docker-compose.yml up -d --remove-orphans

docker exec -it containers_db_1 bash

docker exec -it containers_pgbouncer_1 bash
