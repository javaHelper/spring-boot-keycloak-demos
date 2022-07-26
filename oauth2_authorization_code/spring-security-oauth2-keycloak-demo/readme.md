# spring-security-oauth2-keycloak-demo

Make sure keycloak is up. Follow: https://www.keycloak.org/getting-started/getting-started-docker

`docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin quay.io/keycloak/keycloak:18.0.2 start-dev`

This will start Keycloak exposed on the local port 8080. It will also create an initial `admin` user with username `admin` and password `admin`.

Docker:

```sh
user@Prateeks-MacBook-Pro spring-boot-keycloak-demos % docker ps
CONTAINER ID   IMAGE                                   COMMAND                  CREATED        STATUS                  PORTS                                    NAMES
dfee46d0ab26   quay.io/keycloak/keycloak:18.0.0        "/opt/keycloak/bin/k…"   6 weeks ago    Up 3 hours              0.0.0.0:8080->8080/tcp, 8443/tcp         tender_bouman
```

<img width="1059" alt="Screenshot 2022-07-26 at 3 00 32 PM" src="https://user-images.githubusercontent.com/54174687/180974119-7e7a58bd-9756-4ad4-9e11-fece526929d2.png">

Then click on clients

<img width="1215" alt="Screenshot 2022-07-26 at 3 02 25 PM" src="https://user-images.githubusercontent.com/54174687/180974362-481b25bc-fa67-4d69-964a-e4b5db96fa8b.png">
<img width="869" alt="Screenshot 2022-07-26 at 3 02 39 PM" src="https://user-images.githubusercontent.com/54174687/180974396-d97bf193-bc8b-4ebe-98ae-45976c431e17.png">

- Create User prateek and populate required information and set the password permanent.

- URL to get more info - http://localhost:8080/realms/oauth2-demo-realm/.well-known/openid-configuration

application.properties

```properties
server.port=8090

spring.security.oauth2.client.registration.oauth2-demo-thymeleaf-client.client-id=oauth2-demo-thymeleaf-client
spring.security.oauth2.client.registration.oauth2-demo-thymeleaf-client.client-secret=U50tLvpHlrS8PH30ymCXFV45lXNHlLDG
spring.security.oauth2.client.registration.oauth2-demo-thymeleaf-client.scope=openid, profile, roles,email,address
spring.security.oauth2.client.registration.oauth2-demo-thymeleaf-client.authorization-grant-type=authorization_code
spring.security.oauth2.client.registration.oauth2-demo-thymeleaf-client.redirect-uri=http://localhost:8090/login/oauth2/code/oauth2-demo-thymeleaf-client

spring.security.oauth2.client.provider.oauth2-demo-thymeleaf-client.issuer-uri=http://localhost:8080/realms/oauth2-demo-realm
```

http://localhost:8090/home you should see below

<img width="408" alt="Screenshot 2022-07-26 at 3 07 28 PM" src="https://user-images.githubusercontent.com/54174687/180975329-71091a12-e9aa-4a50-9add-c75422f24bb6.png">
