FROM rgoyard/apache-proxy

RUN set -x \
  && cd /etc/apache2/mods-available \
  && sed -i -s '/^SSLMutex/s/^/#/' ssl.conf \
  && cd /etc/apache2/mods-enabled \
  && ln -s ../mods-available/ssl.* . \
  && echo Done.

VOLUME /auth /cert /etc/apache2/conf.d

EXPOSE 80 443
