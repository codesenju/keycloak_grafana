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
# Configure Keycloak
- ## Create realm *demo*
- ## Create user
- ## Create client grafana:
![client](media/client.jpg)
- ## Copy secret to grafana config file:
![secret](media/secret.jpg)
![grafana_config](media/grafana_config.jpg)

- ## Create Roles:
![role_1](media/create_role_1-2.jpg)
![role_2](media/create_role_3-4.jpg)
![role_3](media/create_role_final.jpg)

- ## Create group(s) & Group mappings:
![mappings_1](media/group_mapping_1-2.jpg)
![mappings_2](media/group_mapping_3-4.jpg)
![group_created](media/group_created.jpg)
![mappings_3](media/group_mapping_5-7.jpg)
![mappings_3](media/group_mapping_updated.jpg)
- ## repeat for grafana_editor:
- ## Add User to group
- ## Create Client mappings:
![client_mappings](media/client_mapper.jpg)

# Start grafana
```
docker-compose up -d
```
```
docker-compose ps
```
## Go to [https//localhost:8443](http//localhost:4000)

# Video
![keycloak](media/keycloak.gif)
# References
## Check Realm Endpoints:
```
{{server}}/auth/realms/{{realm}}/.well-known/openid-configuration
```
```
https://localhost:8443/realms/demo/.well-known/openid-configuration
```

