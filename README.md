# Strapi + NuxtJS starter

## Docker

### Setup

```bash
cp .env.dist .env

# Configure your .env file

# Build images and start containers
sudo docker-compose up --build

# After NuxtJS container listening => Ctrl+C
```

### Start containers

```bash
sudo docker-compose start
```

### Access to Strapi container (backend)

```bash
sudo docker exec -it strapi bash
```

### Access to NuxtJS container (frontend)

```bash
sudo docker exec -it nuxt bash
```

### Extra

Tools setted up by default in each container :
- `vi`
- `git`
- `unzip`
- `wget`

## Strapi Admin Panel

[http://localhost:1337/](http://localhost:1337/)

## NuxtJS Application running

[http://localhost:3000/](http://localhost:3000/)

