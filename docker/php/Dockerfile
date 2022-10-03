FROM php:8.1-fpm AS base_app

RUN apt-get update && apt-get install vim -y
RUN curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.deb.sh' | bash
RUN apt-get install symfony-cli -y
RUN symfony check:requirements

FROM base_app AS base_app_dev

