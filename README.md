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

`vim` is installed by default on each container.

It can be usefull if you want to check/edit file in container directly.


## Strapi Admin Panel

[http://localhost:1337/](http://localhost:1337/)

## NuxtJS Application running

[http://localhost:3000/](http://localhost:3000/)

