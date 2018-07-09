# KeycloakAutoLinkAuthenticator
Automatically link brokered identities without any validation with this Keycloak authenticator.  This is useful in an intranet environment of multiple user databases each with overlapping usernames/emails, but different passwords and you want to allow users to use any password without having to validate (this is only reasonable if you manage all internal databases and usernames/emails matching those in another belong to the same person).

This authenticator would be dangerous in a generic environment where users can register themselves using arbitrary usernames / email addresses.  For example, a user could register my username / email address before I got a chance to.  In a work intranet where users are assigned usernames and email addresses and there just happens to be multiple databases where one database contains a subset of users from another this authenticator could work - for example if you trust that user "johndoe" in database A is the same as in database B.  Why do you have multiple databases of duplicate users in the first place? Maybe a legacy system.  Maybe different administrative realms.  Maybe you've just got a strange environment.

## See Also
   - https://www.keycloak.org/
   - https://www.keycloak.org/docs/latest/server_development/index.html#_auth_spi
   - https://issues.jboss.org/browse/KEYCLOAK-7270
