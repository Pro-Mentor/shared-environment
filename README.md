# Shared Environment

## start the instace

```
    docker compose up
```

- setup keycloak
- setup postgres

## setup local development environment

- add following lines to the _hosts_ files

  - in windows (usually in C:\Windows\System32\drivers\etc\hosts) \
  - in linux base systems (usually in /etc/hosts)

```
127.0.0.1 idp.promentor.local
```

## Go to keycloak admin console

- http://idp.promentor.local:8080/

```
    username: admin
    password: admin
```

### CI/CD

<img src="https://github.com/Pro-Mentor/shared-environment/blob/main/assets/Shared_ENV_Deployment.drawio.png" alt="CI/CD diagram" title="CI/CD Diagram">

## Referances

- set keycloak
  https://keepgrowing.in/tools/
