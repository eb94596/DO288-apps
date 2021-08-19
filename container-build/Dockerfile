# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

RUN chgrp -R 0 ${DOCROOT}/ && \
    chmod -R g=u ${DOCROOT}/
EXPOSE 8080
USER 1001

