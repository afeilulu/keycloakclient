# keycloakclient
Spring boot + keycloak

# run keycloak as docker
```
docker run -p 8080:8080 -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin quay.io/keycloak/keycloak:9.0.2
```

1. login in keycload as admin:admin
2. register your realm, such as "nroad"
3. create "user" role and assign it to user "user1"
4. specify "valid redirect url" for authtication

# prepare a temporary db
```
java -cp ./lib/hsqldb.jar org.hsqldb.server.Server --database.0 file.testdb --dbname.0 testdb
```

# run application