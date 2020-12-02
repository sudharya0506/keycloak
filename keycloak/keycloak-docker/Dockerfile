FROM quay.io/keycloak/keycloak
###ADD dns_ping.cli /opt/jboss/tools/cli/jgroups/discovery/
COPY ./default.cli /opt/jboss/tools/cli/jgroups/discovery/default.cli
ADD standalone-ha.xml /opt/jboss/keycloak/standalone/configuration/
CMD ["-b", "0.0.0.0", "--server-config", "standalone-ha.xml"]
