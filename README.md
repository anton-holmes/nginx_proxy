# nginx_proxy
nginx_proxy


docker run -d -p 9001:9000 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer:latest

docker run -itd --name nginx -p 8080:80 -v ./nginx.conf:/etc/nginx/nginx.conf -v ./defauil.conf:/etc/nginx/conf.d nginx:latest
