# Dockerails
Dockersize for multi project Rails


### Environment
- Ruby: 2.7.1
- MySQL 5.7
### Config database

```yml
  username: <%= ENV['DB_USERNAME'] %>
  password: <%= ENV['DB_PASSWORD'] %>
  port: <%= ENV['DB_PORT'] %>
  host: <%= ENV['DB_HOST'] %>
  database: <%= ENV['DB_NAME'] %>
  socket: /var/run/mysqld/mysqlx.sock
 ```
### Run: 
 - docker-composer build
 - docker-compose run api bundle install
 - docker-compose run admin bundle install
 - docker-compose up -d
