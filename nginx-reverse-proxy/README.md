# nginx-reverse-proxy
docker run -itd --name nginx -p 8081:80 -v ./nginx:/etc/nginx -e VIRTUAL_HOST=server.ais nginx:latest


-e VIRTUAL_HOST=server.ais


docker run -it -d \
    -p 8080:8080 \
    -p 53:53 \
    -p 53:53/udp \
    -v /somefolder:/var/cache/bind \
    -v /someotherfolder:/root/database \
    -e DDNS_ADMIN_LOGIN=admin:123455546. \
    -e DDNS_DOMAINS=dyndns.example.com \
    -e DDNS_PARENT_NS=ns.example.com \
    -e DDNS_DEFAULT_TTL=3600 \
    -e VIRTUAL_HOST=server.ais \
    --name=dyndns \
    bbaerthlein/docker-ddns-server:latest

    http://admin:123455546.@dyndns.example.com/update?hostname=ais.dyndns.example.com