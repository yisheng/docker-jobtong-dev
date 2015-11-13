FROM yangdesheng/php56

# PHP Extensions
RUN yum install -y \
    php56-php-pecl-gearman \
    supervisor

ADD gearman-consumer.ini /etc/supervisord.d/

CMD ["supervisord", "-n"]