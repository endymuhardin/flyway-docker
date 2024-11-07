# Menjalankan Migrasi Flyway dengan Docker #

1. Jalankan dulu database MySQLnya

    ```
    docker compose up
    ```

2. Jalankan migrasi

    ```
    docker run --rm -v ${PWD}/flyway:/flyway/project flyway/flyway migrate -workingDirectory="project"
    ```