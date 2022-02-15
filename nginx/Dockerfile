FROM nginx
RUN apt-get update \
    && apt-get install -y --no-install-recommends net-tools nano \
    && apt-get -y clean \
    && rm -rf /var/lib/apt/lists/*
COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./default.conf /etc/nginx/ssl/conf.d/default.conf
COPY ssl/server.crt /etc/nginx/ssl/server.crt
COPY ssl/server.key /etc/nginx/ssl/server.key
