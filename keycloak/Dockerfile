FROM quay.io/keycloak/keycloak:21.1.2
ARG KC_CLIENT_SECRET
COPY ./realm-export.json /opt/keycloak/data/import/realm-export.json
COPY --chmod=+x --chown=keycloak:keycloak ./custom-health-check.sh /opt/keycloak/custom-health-check.sh