# How to start with integration

- Experiments can start with [Docker](https://www.docker.com/technologies/overview) containers:
    + Clone the repository [yemon](https://github.com/geobeyond/yemon.git) for prototyping. More on such name later
    ```bash
    docker-compose up #you are starting both geoserver and openam
    ```
    + Set this configuration in your docker host machine:
        ```conf
        <$DOCKER_HOST>   openam     openam.example.com
        <$DOCKER_HOST>   geoserver  geoserver.example.com
        ```
- **OpenAM** UI available at [http://openam.example.com:8080/openam](http://openam.example.com:8080/openam)
- **GeoServer** UI available at [http://geoserver.example.com:9000/geoserver](http://geoserver.example.com:9000/geoserver)
- Configure your authN and authZ policies from the GUI console
