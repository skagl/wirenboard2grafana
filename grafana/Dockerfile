FROM grafana/grafana:9.0.3-ubuntu
COPY ./config/grafana.ini /etc/grafana/grafana.ini

USER root

RUN mkdir /var/lib/grafana_plugins
RUN grafana-cli --pluginsDir=/var/lib/grafana_plugins plugins install natel-influx-admin-panel

USER 472