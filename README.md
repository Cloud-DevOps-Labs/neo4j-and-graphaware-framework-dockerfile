# Dockerfile: Neo4j + GraphAware

- launch.sh is copied from [neo4j's offical Dockerfile repo](https://github.com/neo4j/docker-neo4j-publish/blob/a50bed8c92cb9d24adb6b5a7353455c222b1be9d/3.1.3/community/docker-entrypoint.sh) and silghtly modified
- Dockerfile is a merge from [neo4j's offical Dockerfile repo](https://github.com/neo4j/docker-neo4j-publish/blob/a50bed8c92cb9d24adb6b5a7353455c222b1be9d/3.1.3/community/Dockerfile) and [Pelirrojo's work back from 2015](https://github.com/Pelirrojo/neo4j-and-graphaware-framework-dockerfile/blob/2.2/Dockerfile)
- graphaware download list is getting from [is's community download list](https://products.graphaware.com/?dir=framework-server-community)

## Add more plugins

Just add wget xxx after comment ```# add graphaware``` in Dockerfile, and don't forget the ``` && \``` after each line!
