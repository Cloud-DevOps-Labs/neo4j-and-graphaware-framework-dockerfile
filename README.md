[![Docker Automated buil](https://img.shields.io/docker/automated/jrottenberg/ffmpeg.svg)](https://hub.docker.com/r/pelirrojo/neo4j-and-graphaware-framework)
[![Docker Build Statu](https://img.shields.io/docker/build/pelirrojo/neo4j-and-graphaware-framework.svg)](https://hub.docker.com/r/pelirrojo/neo4j-and-graphaware-framework)

# Dockerfile: Neo4j + GraphAware

Neo4j is a highly scalable, robust (fully ACID) native graph database. Neo4j is used in mission-critical apps by thousands of leading, startups, enterprises, and governments around the world. With this Dockerfile and it's DockerHub repository you've a  neo4j 3.1.3 community edition image with [Graphaware Frameworks](https://github.com/graphaware/neo4j-framework) and [WarmUp](https://github.com/graphaware/neo4j-warmup) plugins ready to go.

## Using by pulling from [DockerHub](https://hub.docker.com/r/pelirrojo/neo4j-and-graphaware-framework)

You can view all the versions in different branches of current repo:

* Neo4j@[3.1.3](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/3.1.3/Dockerfile) based on: [openjdk:8-jre-alpine](https://hub.docker.com/r/library/openjdk/tags/8-jre-alpine/)
* Neo4j@[2.2](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/2.2/Dockerfile) based on: [java:latest](https://hub.docker.com/r/library/java/tags/latest/)
* Neo4j@[2.1.7](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/2.1.7/Dockerfile) based on: [java:latest](https://hub.docker.com/r/library/java/tags/latest/)
* Neo4j@[2.1.6](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/2.1.6/Dockerfile) based on: [java:latest](https://hub.docker.com/r/library/java/tags/latest/)

```bash
  $ docker run -it -p {ports} pelirrojo/neo4j-and-graphaware-framework:${version}
  
  i.e.
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework:3.1.3
  
```

and then open [http://localhost:7474](http://localhost:7474) in your browser or use the different API endpoints at:
* Neo4j Native: [http://localhost:7474/db/data/](http://localhost:7474/db/data/)
* GraphAware: [http://your-neo4j-url:7474/graphaware/count](http://your-neo4j-url:7474/graphaware/count)

Note:
Be careful because there are several changes in the API and in the response format between different versions.

## Development and testing

In order to *build* use:
```bash
  $ docker build -t neo4j-graphaware .
```

## Contribute

Feel free to make any further modifications and/or PR :)

## Thanks

Thanks to [tpires](https://github.com/tpires) for its original [repo](https://github.com/tpires/neo4j) and [linonetwo](https://github.com/linonetwo) for pumping version and several improvements 
