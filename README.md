# greenlight_ldap_resync
Python Script to resync the fullnames to the greenlight database from a given LDAP-database.

It fetches all users from LDAP and tries to update them in greenlight's postgres database.


# Information

```python
psql_data = "host=localhost dbname=greenlight_production user=postgres password=PG-PASS" 
```

PG-PASS is the password, that is set as DB_PASSWORD in the .env file of greenlight.
