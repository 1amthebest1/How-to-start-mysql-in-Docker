//download the image via `docker pull mysql:latest` OR `docker pull mysql:versionNumber`

//build and run via `docker run --name mysql-container -d -p 3306:3306 -v /home/{path where you want the db of the container to be}:/var/lib/mysql -e MYSQL_ROOT_PASSWORD={yourPassword} {imageName}` 

//then create a bash shell on the container by using `docker exec -it {container id} /bin/bash` OR login from the box using `mysql -h 127.0.0.1 -P 3306 -u root -p `

//login to the mysql server via `mysql -u root -p`

//enter `create user 'testUser'@'localhost' identified by 'testPass';`

//enter `create database testDatabase;`

//enter `use testDatabase;`

//enter `create table users (email varchar(255), password varchar(255));`

//enter `GRANT INSERT, SELECT, DELETE ON .* TO 'testUser'@'localhost';`

//enter `flush privileges;`

//enter `exit;` to exit out of the mysql server
