### How to set enviroment in bash script using .env file
    #!/usr/bin/env bash
    set -o allexport
    source .env
    set +o allexport