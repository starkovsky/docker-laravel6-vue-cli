FROM php:7.3-fpm

ENV http_proxy ${HTTP_PROXY}
ENV https_proxy ${HTTPS_PROXY}

RUN apt-get update


# POSTGRES SQL
ARG PDO_POSTGRESQL=false
RUN if [ ${PDO_POSTGRESQL} = true ]; then \
    docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql \
    && docker-php-ext-install pdo pdo_pgsql pgsql \
;fi
