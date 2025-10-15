# Docker Redis Dev Image Demo

This mini-project demonstrates a ready-to-use Redis development container using Docker Compose. It sets up Redis 7 with a password and persistent volume.

## Description
- **docker-compose.yml**: Configuration for Redis service with command for password protection.
- **Ports**: Maps Redis port 6379 for external access.
- **Volumes**: Persists data in redis_data volume.

## Instructions
1. Install Docker and Docker Compose.
2. Run: `docker-compose up -d` to start the container.
3. Connect to Redis: `redis-cli -h localhost -p 6379 -a devpass`
4. Stop: `docker-compose down`.

Extend this by adding Redis Sentinel, Cluster, or connecting to an application with redis-py or ioredis.