# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 ${DOCROOT}/ && \
    chmod -R g=u ${DOCROOT}/
EXPOSE 8080
USER 1001

