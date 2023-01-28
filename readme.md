# Wordpress Development Environment

This can be used as a starting place for local Wordpress theme/plugin development.

## Features

- Fully dockerized & repeatable.
- Properly supports custom port (no redirect issues).
- Uses [SQLite plugin](https://github.com/aaemnnosttv/wp-sqlite-db) for faster startup & load times.
- Only exposes `/wp-content` folder for more focused development.

## Prerequisites

- [Docker](https://www.docker.com/products/docker-desktop/)

## Setup

1. Duplicate `example.env` as `.env`

## Startup

1. Run `docker-compose up`
2. Go to http://localhost:3000

## To change port:

1. Edit `docker-compose.yml` file to replace all occurances of default port `3000` with desired port.
2. Re-build container by running `docker-compose build --no-cache`.