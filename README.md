docker-ubuntu-hhvm-nginx
========================

Image for docker with Ubuntu Trusty, HHVM, NGINX and Supervisord

##Docker DNS Issue #541

[ Containers cannot resolve DNS if docker host uses 127.0.0.1 as resolver](https://github.com/docker/docker/issues/541)

[Google Public DNS](https://developers.google.com/speed/public-dns/docs/using?hl=nl)

    sudo sh -c "echo 'DOCKER_OPTS=\"-dns 8.8.8.8 -dns 8.8.4.4\"' > /etc/default/docker"

For DOCKER_OPTS see also [Docker Advanced networking TL;DR](https://docs.docker.com/articles/networking/)

## Partial fork from:

[Dockerfiles](https://github.com/Joostvanderlaan/dockerfiles/tree/master/ubuntu14/baseimage-nginx-hhvm)
by Joost van der Laan

