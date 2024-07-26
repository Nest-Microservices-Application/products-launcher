## Dev

1. Clone repository
2. Config `.env` variables based on `.env.template`
3. Run `git submodule update --init --recursive` to rebuild the submodules
4. Start docker containers building `docker compose up --build`

## Prod

1. Build images running `docker compose -f docker-compose.prod.yml build`
2. Run containers running `docker compose -f docker-compose.prod.yml up`
