# Running RethinkDb in container

Use one of the following container engine to run the provided compose file to run `rethinkDB`.

## Podman

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
    podman logs -f rethink_rethinkdb_1
    ```

## Rancher

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

## Docker

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
