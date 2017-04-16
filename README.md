# Dockerfile: Neo4j + GraphAware

Neo4j is a highly scalable, robust (fully ACID) native graph database. Neo4j is used in mission-critical apps by thousands of leading, startups, enterprises, and governments around the world. With this Dockerfile and it's DockerHub repository you've a  neo4j 3.1.3 community edition image with [Graphaware Frameworks](https://github.com/graphaware/neo4j-framework) and [WarmUp](https://github.com/graphaware/neo4j-warmup) plugins ready to go.

## Using by pulling from [DockerHub](https://hub.docker.com/r/pelirrojo/neo4j-and-graphaware-framework/)

You can view all the versions in different branches of current repo

```bash
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework:3.1.3
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework:2.2
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework:2.1.7
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework:2.1.6
```
and then open (http://localhost:7474)[http://localhost:7474] in your browser or use the API endpoint at:
* Neo4j Native: [http://localhost:7474/db/data/](http://localhost:7474/db/data/)
* GraphAware: [http://your-neo4j-url:7474/graphaware/count](http://your-neo4j-url:7474/graphaware/count)

Note:
Be careful because there are several changes in the API and in the response format between different versions.

## Development and testing

In order to *build* use:
```bash
  $ docker build -t neo4j-graphaware .
```

## Contribute

Feel free to make any further modifications and/or PR :)

## Thanks

Thanks to [tpires](https://github.com/tpires) for its original [repo](https://github.com/tpires/neo4j) and [linonetwo](https://github.com/linonetwo) for pumping version and several improvemnts 
