ARG CF_SRC_OS_IMAGE

FROM ${CF_SRC_OS_IMAGE}

ARG CF_CPUARCH_DEB_DIST

ARG CF_MAILHOG_VERSION

ADD files/mailhog-${CF_MAILHOG_VERSION}-${CF_CPUARCH_DEB_DIST}.tgz /opt/

ENV PATH=$PATH:/opt/mailhog-${CF_MAILHOG_VERSION}-${CF_CPUARCH_DEB_DIST}

RUN \
	groupadd -g 1000 mailhog \
	&& useradd -u 1000 -g 1000 -m mailhog \
	&& cp /root/.bashrc /home/mailhog/ \
	&& chown mailhog:mailhog /home/mailhog/

WORKDIR /home/mailhog

USER mailhog
ENV HOME=/home/mailhog

ENTRYPOINT ["MailHog"]

# Expose the SMTP and HTTP ports:
EXPOSE 1025 8025
