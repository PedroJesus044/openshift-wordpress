FROM ubi8/php-74

ADD wordpress* .
RUN unzip wordpress* -d ..
USER 0

RUN chgrp -R 0 /opt/app-root/src && \
    chmod -R g=u /opt/app-root/src

WORKDIR /opt/app-root/src


CMD /usr/libexec/s2i/run