FROM nginx:alpine

ENV http_proxy ${HTTP_PROXY}
ENV https_proxy ${HTTPS_PROXY}

ADD ./sites/host.conf /etc/nginx/conf.d/default.conf
