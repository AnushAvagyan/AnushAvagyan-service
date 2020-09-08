# Project Name

> Microservice responsible for managing, storing and displaying data related to the property hosts.

## Related Projects

  - https://github.com/RPT20-FEC/listing-service
  - https://github.com/RPT20-FEC/similarprops-service
  - https://github.com/RPT20-FEC/photo-service

## Table of Contents

1. [Requirements](#requirements)
1. [Development](#development)
1. [Production](#production)
1. [API](#API)


## Requirements

An `nvmrc` file is included if using [nvm](https://github.com/creationix/nvm).

- Node 12.16.2
- MongoDB
- React
- Webpack


## Installing Dependencies

From within the root directory

```sh
npm install -g webpack
npm install
```

## Development

For development mode this project uses nodemon and webpack watching for changes

```sh
npm run react:dev
npm start
npm run test 
```

## Production
For production mode this project uses webpack in production

```sh
npm run build
npm start
```
## API

- GET /host/:id - return JSON object of property host data based on the user id

- GET /hosts/:id/co-hosts - returns a JSON object of cohost data for a specific host

- GET /listings/:id/hosts - returns a JSON object of host data based on the property id

- POST /hosts - creates a new user in the hosts table

- PUT /hosts/:id - updates host data for the host with matching host id

- DELETE /hosts/:id - deletes the record from database that belongs to the host with matching host id

