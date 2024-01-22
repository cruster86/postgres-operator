Апстрим проект: https://github.com/zalando/postgres-operator.git

Сборка образа из апстрим проекта: `docker build -t registry.sirius.online/infra/postgres-operator:latest -f docker/Dockerfile .`

docker/Dockerfile:

  - `ARG BASE_IMAGE=alpine:latest`

docker/build_operator.sh:

  - `wget -q "https://storage.googleapis.com/golang/go1.21.1.linux-${arch}.tar.gz" -O go.tar.gz`