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

- http://idp.promentor.local/

```
    username: admin
    password: admin
```

- go to <b>Users</b> and set admin account email in master realm

- select the relevant realms from top left drop down and go to <b>Realm Settings</b> -> <b> Email</b> Tab.

- In the <b>Connection & Authentication</b> section first <i>Disable</i> the <b>Authentication</b> and then <i>Enable</i> it.

- Replace the <b>Password</b> with the SMTP server access key and <b>Save</b> it and click on <b>Test Connection</b> to test the connection

### CI/CD

<img src="https://github.com/Pro-Mentor/shared-environment/blob/main/assets/Shared_ENV_Deployment.drawio.png" alt="CI/CD diagram" title="CI/CD Diagram">

## Referances

- set keycloak
  https://keepgrowing.in/tools/
