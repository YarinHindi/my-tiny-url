# tinyurl

REST API web service written in Spring-Boot (Java), allows users to short URLs, monitor, track after them, and see statistics.

# How to run
1. Make sure you have docker install on your machine
2. Clone the project:
```
git clone git@github.com:YarinHindi/my-tiny-url.git
```
3. Go to the project directory
4. Start docker-compose
```
docker-compose up -d
```
5. To create cassandra key space you may need to run this command before on the cassandra machine
```
CREATE KEYSPACE tiny_keyspace
WITH replication = {'class':'SimpleStrategy', 'replication_factor' : 1};
```
6. After starting the server you can use the swagger on this adress:
```
http://localhost:8080/swagger-ui.html#
```
