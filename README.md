# greenlight_ldap_resync
Python Script to resync the fullnames to the greenlight database from a given LDAP-database.

It fetches all users from LDAP and tries to update them in greenlight's postgres database.


# Information
These variables need to be adjusted.

```python
ldap_server = "ldaps://yourcompany.com:636"
basedn = "ou=people,dc=company,dc=de"
binddn = "cn=your_user,ou=admin,dc=company,dc=de"
pw = ""
psql_data = "host=localhost dbname=greenlight_production user=postgres password=PG-PASS" 
```

pw is the password of your ldap user (binddn).

PG-PASS is the password, that is set as DB_PASSWORD in the .env file of greenlight.
