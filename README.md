# Errbit LDAP

this is a fork of https://github.com/errbit/errbit with added LDAP authentication support.

  * added devise_ldap_authenticatable gem
  * ldap only authentication
  * ldap settings configurable by env vars
  * authenticate by username
  * password recovery removed
  * create user at first ldap login

# usage

## environment variables

| Name | Description / Example | Default |
| --- | --- | --- |
| LDAP_GROUP_BASE | ldap group base / ou=groups,dc=acme,dc=com | - |
| LDAP_REQUIRED_GROUP |  the group the users have to be part of for accessing errbit / cn=errbit,ou=groups,dc=acme,dc=com | - |
| LDAP_HOST | ldap server host | localhost |
| LDAP_PORT | ldap server port | 636 |
| LDAP_BASE | ldap user base / ou=users,dc=acme,dc=com | - |
| LDAP_SSL | ldap ssl mode | simple_tls |
| LDAP_USER_ATTR | ldap user attribute to identify user | cn |

# links

  * https://github.com/cschiewek/devise_ldap_authenticatable

