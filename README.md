# Spring Boot 3.0 – JWT Authentication with Spring Security using MySQL Database

## References :- 

- [GeeksforGeeks](https://www.geeksforgeeks.org/spring-boot-3-0-jwt-authentication-with-spring-security-using-mysql-database/)

## Steps

- run this docker file for mysql database in docker
- create a database in mysql with name springSecurity


content for docker compose file - for running mysql in docker


```yml
# Use root/example as user/password credentials
version: '3.1'

services:

  db:
    image: mysql
    # NOTE: use of "mysql_native_password" is not recommended: https://dev.mysql.com/doc/refman/8.0/en/upgrading-from-previous-series.html#upgrade-caching-sha2-password
    # (this is just an example, not intended to be a production configuration)
    ports:
      - 3306:3306
    command: --default-authentication-plugin=mysql_native_password
    restart: always
    environment:
      MYSQL_ROOT_PASSWORD: example
  # adminer:
  #   image: adminer
  #   restart: always
  #   ports:
  #     - 8080:8080

# run 
# docker-compose up - on windows
# docker compose up - on linux
```

```sh
echo "# jwt-with-spring-security-mysql" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/adityasuman100/jwt-with-spring-security-mysql.git
git push -u origin main
```

```sh
git remote add origin https://github.com/adityasuman100/jwt-with-spring-security-mysql.git
git branch -M main
git push -u origin main
```