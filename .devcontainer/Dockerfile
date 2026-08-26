FROM sibedge/postgres-plv8:latest

USER root

# Install OpenSSH, bash, sudo, and GNU utility replacements for BusyBox
RUN apk update && apk add --no-cache \
    openssh \
    openssh-server \
    bash \
    sudo \
    shadow \
    coreutils \
    findutils \
    grep \
    curl \
    && ssh-keygen -A \
    && mkdir -p /var/run/sshd /var/empty \
    && chmod 755 /var/empty
