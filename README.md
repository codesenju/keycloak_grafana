# Setup
### Create network keycloak_net:
```
docker network create keycloak_net
```
### Spin up containers:
```bash
docker-compose up -d keycloak
```
### Go to [https//localhost:8443](https//localhost:8443)
</br>



### Check Realm Endpoints:
```
{{server}}/auth/realms/{{realm}}/.well-known/openid-configuration
```
```
https://localhost:8443/realms/demo/.well-known/openid-configurationhttps://localhost:8443/realms/Demo/.well-known/openid-configuration
```

```
docker-compose up -d
```


# Video
![keycloak](media/keycloak.gif)