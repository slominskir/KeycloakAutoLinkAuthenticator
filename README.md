# KeycloakAutoLinkAuthenticator
Automatically link brokered identities without any validation with this Keycloak authenticator.  This is useful in an intranet environment of multiple user databases each having duplicate usernames/emails, but different passwords and you want to allow users to use either password without having to validate (this is only reasonable if you manage all internal databases and there is a one-to-one mapping of usernames/emails between databases).

## See Also
   - https://www.keycloak.org/
   - https://www.keycloak.org/docs/latest/server_development/index.html#_auth_spi
   - https://issues.jboss.org/browse/KEYCLOAK-7270
