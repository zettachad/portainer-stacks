## Notes to self

- create the required directories as root user
  ```
  mkdir -p /docker-compose-core-stack/
  chmod 744 /docker-compose-core-stack
  ```
- add the output from the following command to env
  ```
  htpasswd -n myusername
  ```
- your env should look like this
  ```
  DOMAIN=kush.in
  HOSTNAME=yourhostname
  TRAEFIK_USERS='myusername:$apr1$tB7jbznW$IH0wShSpEJ6xUJnKL4JjQ'
  ACME_EMAIL='xyz@example.com'
  ```
- change volume mappings in compose files if server was changed
