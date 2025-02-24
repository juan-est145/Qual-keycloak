FROM keycloak/keycloak:26.0

WORKDIR /opt/keycloak

RUN mkdir -p /opt/keycloak/data/import

COPY 1740134194447-example-realm.json /opt/keycloak/data/import

EXPOSE 8080

ENTRYPOINT ["/opt/keycloak/bin/kc.sh"]

CMD ["start-dev", "--import-realm"]
