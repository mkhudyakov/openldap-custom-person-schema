### 1. Create an environment
```
docker-compose up -d
```

### Import data to OpenLDAP server
```
docker exec ${container_name} ldapadd -x -H ldap://localhost -D "CN=admin,DC=company,DC=com" -f /users.ldif -w admin
```

### Delete an environment
```
docker-compose down
```