# MongoDB Docker Setup for Development and Testing of Lottie Application

## Description

This repository contains a Docker Compose setup for running MongoDB locally. It is intended for use in development and testing environments. This setup provides a simple way to run a MongoDB instance using Docker.

## Prerequisites

- Docker
- Docker Compose

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/chrisdoctor/lottie-mongo-container
   cd lottie-mongo-container
   ```

2. Start MongoDB using Docker Compose:

   ```bash
   docker-compose up -d
   ```

## Docker Compose Configuration

The `docker-compose.yml` file contains the following configuration:

```yaml
version: "3.1"

services:
  mongo:
    image: mongo:latest
    ports:
      - 27017:27017
    environment:
      MONGO_INITDB_ROOT_USERNAME: root
      MONGO_INITDB_ROOT_PASSWORD: password
```

## Usage

### Starting MongoDB

To start the MongoDB service, run:

```bash
docker-compose up -d
```

### Stopping MongoDB

To stop the MongoDB service, run:

```bash
docker-compose down
```
