FROM yangdesheng/php56

RUN yum install -y cronie

# Crontab
ADD crontab.conf /opt/
RUN crontab /opt/crontab.conf

# Start Cron Daemon
CMD ["crond", "-n"]