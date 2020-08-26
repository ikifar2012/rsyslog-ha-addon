FROM hassioaddons/debian-base:3.2.2
SHELL ["/bin/bash", "-o", "pipefail", "-c"]
# Install Components
RUN apt-get update && apt-get install -y rsyslog
# Copy data for add-on
COPY rootfs /
RUN chmod +x rsyslog.sh
RUN chmod +x /etc/services.d/rsyslog/*
# CMD [ "./run.sh" ]