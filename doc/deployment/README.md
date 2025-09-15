# Running RethinkDb in container

Use the following command to run rethinkDb as services using the provided docker compose file.

## Installation with Podman

* Starting the rethinkDB container

    ```bash
    podman-compose -f podman-compose-rethinkdb.yml -p rethink up -d
    ```

* Stopping the rethinkDB container

    ```bash
    podman-compose -f podman-compose-rethinkdb.yml -p rethink stop
    podman-compose -f podman-compose-rethinkdb.yml -p rethink down
    ```

* Checking the rethinkDB container log

    ```bash
    podman logs -f rethink-rethinkdb-1
    ```

## Installation with Rancher

* Starting the rethinkDB container

    ```bash
    nerdctl compose -f docker-compose-rethinkdb.yml -p rethink up -d
    ```

* Stopping the rethinkDB container

    ```bash
    nerdctl compose -f docker-compose-rethinkdb.yml -p rethink stop
    nerdctl compose -f docker-compose-rethinkdb.yml -p rethink down
    ```

* Checking the rethinkDB container log

    ```bash
    nerdctl logs rethink-rethinkdb-1 -f
    ```

## Installation with Docker

* Starting the rethinkDB container

    ```bash
    docker compose -f docker-compose-rethinkdb.yml -p rethink up -d
    ```

* Stopping the rethinkDB container

    ```bash
    docker compose -f docker-compose-rethinkdb.yml -p rethink stop
    docker compose -f docker-compose-rethinkdb.yml -p rethink down
    ```

* Checking the rethinkDB container log

    ```bash
    docker logs rethink-rethinkdb-1 -f
    ```

