FROM php:7.0-fpm
MAINTAINER Amarnath Arora <amarnath.arora@oodlestechnologies.com>

RUN docker-php-ext-install mysqli \
    && apt-get update \
    && apt-get install -y -q --no-install-recommends \
        ssmtp \
    && apt-get clean \
    && rm -r /var/lib/apt/lists/*
