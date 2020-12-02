# dockerTutorial
Instructions covers both the old and new docker commands

## COMMANDS
1. Get the version of the docker client and server (daemon)
    ```
    docker version
    ```

2. Get the detail information on the docker client and server
    ```
    docker info
    ```

3. Start nginx container with `webhost` name
    ```
    docker container run --publish 80:80 --detach --name webhost nginx          # docker run -p 80:80 -d --name webhost nginx
    ```

4. Check the log of a specific container
    ```
    docker container logs -f <container name>       # docker logs -f <container id>
    ```

5. Get a list of active running containers
    ```
    docker container ls         # docker ps
    ```

6. Get a list of both active and inactive containers
    ```
    docker container ls -a      # docker ps -a
    ```

5. Check the top processes running in a specific container
    ```
    docker container top <container name>
    ```