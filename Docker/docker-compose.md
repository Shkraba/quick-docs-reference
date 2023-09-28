
# Docker Compose
 Docker Compose is a tool for defining and running multi-container Docker applications. It allows you to specify your application's services, networks, and volumes in a single file.

## Basic Commands

- `docker-compose up`: Start containers defined in `docker-compose.yml`.
- `docker-compose down`: Stop and remove containers, networks, and volumes.
- `docker-compose up -d`: Start containers in detached mode.
- `docker-compose ps`: List running containers.
- `docker-compose logs`: View container logs.

## Compose File

- `docker-compose -f <file>`: Specify a different Compose file (e.g., `docker-compose -f custom-compose.yml`).
- `docker-compose config`: Validate and view the merged Compose file.
- `docker-compose build`: Build or rebuild services.
- `docker-compose pull`: Pull service images from the registry.

## Service Management

- `docker-compose up <service>`: Start a specific service.
- `docker-compose stop <service>`: Stop a specific service.
- `docker-compose restart <service>`: Restart a specific service.
- `docker-compose scale <service>=<count>`: Scale a service to a specific number of containers.

## Environment Variables

- Use `.env` files for environment variables.
- Define variables in the `.env` file (e.g., `VAR=value`).
- Reference variables in the `docker-compose.yml` file (e.g., `${VAR}`).

## Docker-Compose Networking
By default Docker-Compose will create a new network for the given compose file. You can change the behavior by defining custom networks in your compose file.
### Create and assign custom network
...
*Example:*
```yaml
networks:
  custom-network:

services:
  app:
    networks:
      - custom-network
```
### Use existing networks
If you want to use an existing Docker network for your compose files, you can add the `external: true` parameter in your compose file
*Example:*
```yaml
networks:
  existing-network:
    external: true
```

## Volumes
Volumes allow Docker containers to use persistent storage. In a compose file, you can create and map volumes like this:
```yaml
volumes:
  my-volume:

services:
  app:
    volumes:
      - my-volume:/path-in-container
```

These volumes are stored in `/var/lib/docker/volumes`.
