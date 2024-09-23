ARG DOCKER_TAG=${DOCKER_TAG:-latest}

FROM docker.io/nextcloud:{$DOCKER_TAG}

RUN ln -fs /dev/null /var/log/apache2/access.log && \
  ln -fs /dev/null /var/log/apache2/error.log
