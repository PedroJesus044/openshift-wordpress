FROM ubi8/php-74

ADD wordpress* .
USER 0
RUN chgrp -R 0 /wordpress && \
    chmod -R g=u /wordpress
WORKDIR /wordpress

CMD /usr/libexec/s2i/run