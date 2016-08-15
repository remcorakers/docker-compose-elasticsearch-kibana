FROM kibana:latest

# switch users; see issue https://github.com/docker-library/kibana/issues/20
USER kibana
RUN kibana plugin --install elastic/sense
USER root
