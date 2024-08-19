FROM ubi8/php-74

ADD wordpress* .
RUN unzip wordpress* -d ..
USER 0

RUN chgrp -R 0 wordpress && \
    chmod -R g=u wordpress

WORKDIR /opt/app-root/src/wordpress


CMD /usr/libexec/s2i/run