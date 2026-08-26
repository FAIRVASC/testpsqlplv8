FROM sibedge/postgres-plv8:latest

# Install OpenSSH server, bash, and generate host keys
RUN apk update && apk add --no-cache openssh-server bash sudo \
    && ssh-keygen -A \
    && mkdir -p /var/run/sshd
