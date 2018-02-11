# About this repo

**Drupal** optimized image for Solr (based on makuk66 work) with search-api Solr config files for 3.x, 4.x, 5.x, and 6.x.
7.x does not include search-api Solr config files anymore and are just a fork from makuk66.

Available tags are:
- 7.2, latest ([7.2/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/7.2/Dockerfile))
- 7.1 ([7.1/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/7.1/Dockerfile))
- 6.6 ([6.6/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.6/Dockerfile))
- 6.5 ([6.5/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.5/Dockerfile))
- 6.4 ([6.4/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.4/Dockerfile))
- 6.3 ([6.3/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.3/Dockerfile))
- 6.2 ([6.2/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.2/Dockerfile))
- 6.1 ([6.1/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.1/Dockerfile))
- 6.0 ([6.0/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/6.0/Dockerfile))
- 5.5 ([5.5/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.5/Dockerfile))
- 5.4 ([5.4/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.4/Dockerfile))
- 5.3 ([5.3/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.3/Dockerfile))
- 5.2 ([5.2/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.2/Dockerfile))
- 5.1 ([5.1/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.1/Dockerfile))
- 5.0 ([5.0/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/5.0/Dockerfile))
- 4.10 ([4.10/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/4.10/Dockerfile))
- 3.6 ([3.6/Dockerfile](https://github.com/TehesFR/docker-solr/tree/master/3.6/Dockerfile))

# Docker-compose

Please check a complete docker-compose.yml example at: https://github.com/TehesFR/docker-apache-php

[Docker Hub page](https://hub.docker.com/r/tehes/docker-solr/)

# Docker only

If you want to use a standalone docker image, use the following command : 

```
docker run -itd -p 8080:8983 tehes/docker-solr:tag
```
Don't forget to change **tag** by the SolR version you want to use. For SolR 4.10, the command will be : 

```
docker run -itd -p 8080:8983 tehes/docker-solr:4.10
```

# Create a new core

To create a new Solr core, run this command in your Docker container

```
bin/solr create_core -c myCore -p 8983
```
