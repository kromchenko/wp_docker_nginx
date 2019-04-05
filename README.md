# 1. sudo docker-compose up -d
Run the project
# 2. sudo docker-compose stop
Stop the projeckt
# 3.  sudo docker ps
Container status
# 4. sudo docker exec -it
Enter the container
# 5. sudo docker exec -it db bash 
Enter mysql
# 6. mysql -u root -p 
Сonnect to mysql
# 7. show databases;
show all databases
# 8. use yourdb;
Use selected database
№ 9. show tables;
show tables

________________________________________________

- DROP DATABASES your_name_databases; (delete database)
- CREATE DATABASES your_name_databases; (create database)

________________________________________________

# DUMP database

- create a folder in the file docker-compose.yml - ./docker/mysql/:/temp
- reboot - sudo docker-compose stop && sudo docker-compose up -d
- connect to the database - sudo docker exec -it db bash 
- mysqldump-u root -p your_name_databases > /temp/your_name_databases.sql