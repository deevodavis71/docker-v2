# docker-v2

Deploying a registry server

https://docs.docker.com/registry/deploying/#importantrequired-http-headers


Test an insecure registry

https://docs.docker.com/registry/insecure/#deploy-a-plain-http-registry

https://support.symantec.com/en_US/article.TECH242030.html


Listing entries from v2 Repository

curl -k -u testuser:testpassword -X GET https://localhost:5000/v2/rabbitmq/tags/list

curl -k -u testuser:testpassword -X GET https://localhost:5000/v2/rabbitmq/manifests/latest


Deleting Entries from v2 Repo

https://github.com/burnettk/delete-docker-registry-image

export REGISTRY_DATA_DIR=/Users/stevedavis/Downloads/docker_registry/data/docker/registry/v2
./delete_docker_registry_image.py --image testrepo/awesomeimage --dry-run
