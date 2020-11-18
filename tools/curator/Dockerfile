FROM debian:stable-slim

RUN apt -y update;apt -y upgrade; apt install -y python elasticsearch-curator cron tini crond

COPY entrypoint.sh /usr/local/bin/entrypoint
RUN chmod +x /usr/local/bin/entrypoint
ENTRYPOINT ["entrypoint"]
