FROM sameersbn/apt-cacher-ng:latest

RUN set -x \
    && ex -c '/^Port:' -c ':s/3142/80/' -c ':wq' /etc/apt-cacher-ng/acng.conf \
    && echo done.

EXPOSE 80
ENTRYPOINT [ "/sbin/entrypoint.sh" ]
CMD /usr/sbin/apt-cacher-ng -c /etc/apt-cacher-ng
