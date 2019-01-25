# Docker HTTPS Proxy Server (based on Squid 3)
This is a docker image helps you easy deploy secure http/https proxy with login/password authentication

## Install
1. Install ```docker``` and ```docker-compose``` using the instructions from the official website: https://docs.docker.com/install/ and https://docs.docker.com/compose/install/
2. Clone this repo to any directory: ```git clone https://github.com/CaliforniaMountainSnake/docker-https-proxy-server.git```
3. Rename ```.env.example``` file to ```.env``` and set your login, password and proxy port. Additionally you can configure squid in the ```.docker_build_configs/squid/squid.conf```
4. Start proxy server! ```docker-compose up -d```

## Stopping server
Use ```docker-compose down``` to stop proxy server.

## Logs
You can see squid logs in ```containers_files/squid/log/```
