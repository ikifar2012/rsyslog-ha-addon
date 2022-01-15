ARG BUILD_FROM
FROM ${BUILD_FROM}

SHELL ["/bin/bash", "-o", "pipefail", "-c"]

# Install Components
RUN apk add --no-cache rsyslog

# Copy data for add-on
COPY rootfs /
RUN chmod +x rsyslog.sh
RUN chmod +x /etc/services.d/rsyslog/*

# CMD [ "./run.sh" ]