FROM nginx:latest
COPY default.conf /etc/nginx/conf.d/
COPY nginx.conf /etc/nginx/nginx.conf
COPY ./content /usr/share/nginx/html
# ENV VIRTUAL_PORT=80
# ENV VIRTUAL_HOST=project.local
ENTRYPOINT ["/docker-entrypoint.sh"]
CMD ["nginx", "-g", "daemon off;"]


# FROM nginx:alpine

# COPY default.conf /etc/nginx/conf.d/
# COPY nginx.conf /etc/nginx/nginx.conf
# COPY docker-entrypoint.sh /
# RUN chmod +x /docker-entrypoint.sh
# ENV CLIENT_MAX_BODY_SIZE 20M

# ENTRYPOINT ["/docker-entrypoint.sh"]
# CMD ["nginx", "-g", "daemon off;"]
