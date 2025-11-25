After setup see this [docker-compose.yml](./docker-compose.yml)

Run this command:

docker compose up -d

Open your browser and type your IP + port

You should setup in directory: [daemon.json](./daemon.json)

/var/snap/docker/current/config/daemon.json (if using Docker Snap)

/etc/docker/daemon.json (if using standard Docker Engine)

for testing the private registry, you can type:

docker pull nginx

docker tag nginx ur_ip:5000/nginx-custom

docker push ur_ip:5000/nginx-custom
