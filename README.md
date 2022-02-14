
# Keycloak demo

**_More Info on Wiki Page_**

## QuickStart

### Docker compose
Start / logs / refresh / down

```
docker-compose up -d

docker-compose logs -f

docker-compose up --force-recreate --no-deps -d gatekeeper

docker-compose down
```

### Accounts

* Master (keycloak admin): `admin` / `admin`
* User "ADMIN" group: `tony` / `stark`
* User "SIDEKICK" group: `peter` / `parker`

### Network

(hint: [localtest.me](https://readme.localtest.me/) is resolved in 127.0.0.1)

Direct app "demo":
  - direct access: localhost:8180 or localtest.me:8180
  - Docker network: demo:80

Protected app "demo":
  - localtest.me:4180

Keycloak:
  - localtest.me:8080

