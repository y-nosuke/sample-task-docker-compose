# sample-task-docker-compose

## 事前準備

```sh
export DB_USER=task
export DB_PASSWORD=password
export DB_ROOT_PASSWORD=password
export DB_HOST=mysql
export DB_PORT=3306
export DB_DATABASE_NAME=task
export AUTH_JWKS_URL=http://keycloak:8080/realms/sample/protocol/openid-connect/certs
export KEYCLOAK_ADMIN=admin
export KEYCLOAK_ADMIN_PASSWORD=admin
```

`docker\resources\alertmanager\alertmanager.yml.template`をコピーして`alertmanager.yml`を作成し、以下の項目を変更する。

- global.slack_api_url
- receivers.slack_configs.channel