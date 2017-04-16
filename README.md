# Dockerfile: Neo4j + GraphAware

Neo4j is a highly scalable, robust (fully ACID) native graph database. Neo4j is used in mission-critical apps by thousands of leading, startups, enterprises, and governments around the world. With this Dockerfile and it's DockerHub repository you've a  neo4j 3.1.3 community edition image with [Graphaware Frameworks](https://github.com/graphaware/neo4j-framework) and [WarmUp](https://github.com/graphaware/neo4j-warmup) plugins ready to go.

## Setup

In order to *build* use:
```bash
  $ docker build -t neo4j-graphaware .
```
Then do whatever you want with this image.

To directly *pull* you can:

```bash
  $ docker run -it -p 7474:7474 -p 7473:7473 -p 7687:7687 pelirrojo/neo4j-and-graphaware-framework
```

## Add more plugins

* Just add ```wget xxx``` after comment ```# add graphaware``` to [Dockerfile](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/3.1.3/Dockerfile).
*  **Don't** forget the ```&& \``` after each line!

## References

- launch.sh is copied from [neo4j's offical Dockerfile repo](https://github.com/neo4j/docker-neo4j-publish/blob/a50bed8c92cb9d24adb6b5a7353455c222b1be9d/3.1.3/community/docker-entrypoint.sh) and silghtly modified
- Dockerfile is a merge from [neo4j's offical Dockerfile repo](https://github.com/neo4j/docker-neo4j-publish/blob/a50bed8c92cb9d24adb6b5a7353455c222b1be9d/3.1.3/community/Dockerfile) and [Pelirrojo's work back from 2015](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/2.2/Dockerfile)
- graphaware download list is getting from [is's community download list](https://products.graphaware.com/?dir=framework-server-community)

## Thanks

Thanks to [tpires](https://github.com/tpires) for its original [repo](https://github.com/tpires/neo4j) and [linonetwo](https://github.com/linonetwo) for pumping version and several improvemnts 
