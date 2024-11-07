ARG  PHP_VERSION=7.4

FROM phpdockerio/php:${PHP_VERSION}-fpm
WORKDIR "/application"

ENV appname="blog"
ENV versionmajor="1"
ENV versionminor="1"
ENV versionpatch="1"
ENV appversion="v.${versionmajor}.${versionminor}.${versionpatch}"
ENV appauthor="Francisco Abayon"

LABEL name="${appname}" \
      version="${appversion}" \
      author="${appauthor}" \
      description="CurlyBytes Codeigniter 3 upgrades" 


RUN apt-get update \
    && apt-get -y --no-install-recommends install \
        git \
        php${PHP_VERSION}-bcmath \
        php${PHP_VERSION}-bz2 \
        php${PHP_VERSION}-enchant \
        php${PHP_VERSION}-gd \
        php${PHP_VERSION}-gearman \
        php${PHP_VERSION}-gmp \
        php${PHP_VERSION}-grpc \
        php${PHP_VERSION}-http \
        php${PHP_VERSION}-igbinary \
        php${PHP_VERSION}-imagick \
        php${PHP_VERSION}-inotify \
        php${PHP_VERSION}-interbase \
        php${PHP_VERSION}-memcached \
        php${PHP_VERSION}-mongodb \
        php${PHP_VERSION}-mysql \
        php${PHP_VERSION}-oauth \
        php${PHP_VERSION}-odbc \
        php${PHP_VERSION}-pcov \
        php${PHP_VERSION}-phpdbg \
        php${PHP_VERSION}-protobuf \
        php${PHP_VERSION}-pspell \
        php${PHP_VERSION}-psr \
        php${PHP_VERSION}-redis \
        php${PHP_VERSION}-soap \
        php${PHP_VERSION}-sqlite3 \
        php${PHP_VERSION}-ssh2 \
        php${PHP_VERSION}-swoole \
        php${PHP_VERSION}-tidy \
        php${PHP_VERSION}-uuid \
        php${PHP_VERSION}-xdebug \
        php${PHP_VERSION}-xmlrpc \
        php${PHP_VERSION}-yaml \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*
