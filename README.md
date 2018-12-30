# Cassandra

This Apache Cassandra image is based on the standard [library/cassandra](https://hub.docker.com/_/cassandra/) image. 
However, this image will create a default keyspace on boot up.

By default a keyspace named `example` will be created on boot. To change the name you can use the `CASSANDRA_KEYSPACE` 
environment variable.

```Dockerfile
ENV CASSANDRA_KEYSPACE="something"
```

## Usage:

To launch this container run the following

```
docker run madflojo/cassandra
```

This image still supports base image environment variables such as `CASSANDRA_SEEDS`, `CASSANDRA_DC`, etc.

See the [library/cassandra](https://hub.docker.com/_/cassandra/) documentation for base environment variables.
