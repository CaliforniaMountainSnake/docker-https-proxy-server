FROM sameersbn/squid:3.5.27-1

ARG USERNAME
ARG PASSWORD
ARG PASSWORD_FILE=/etc/squid/.htpasswd

RUN apt-get update && apt-get install -y apache2-utils
RUN htpasswd -b -c $PASSWORD_FILE $USERNAME $PASSWORD
