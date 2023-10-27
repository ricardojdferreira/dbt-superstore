FROM apache/superset:77889b29fb0e50473ca7656be4e5bf2f1dff5421
USER root

ENV ADMIN_USERNAME $ADMIN_USERNAME
ENV ADMIN_PASSWORD $ADMIN_PASSWORD

COPY ./superset-init.sh /superset-init.sh
RUN chmod +x /superset-init.sh

USER superset
ENTRYPOINT [ "/superset-init.sh" ]