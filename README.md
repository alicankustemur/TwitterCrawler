# TwitterCrawler

This is a simple **Spring Boot** and **MongoDB** project.
The goal of the project; given **Twitter User** and return this user's friendss' friendship scores.

![TwitterCrawler](https://github.com/alicankustemur/TwitterCrawler/blob/master/src/main/resources/TwitterCrawler.png?raw=true "TwitterCrawler")



## Build
 - Maven
 - JDK 7 or later.

## Dependencies
- Spring Boot Starter MongoDB for MongoDB auto configuration.
- Twitter4J for Twitter API
- Apache Commons Collections 4.1 for Map Operations
- Project Lombok for Domain Model create getter, setter, constructor.


## Requirements

 ### Run
 ```sh
   java -jar TwitterCrawler.jar
   ```
   
  These ones must be installed on your os for run.
  - Maven 
  - MongoDB 
  - JRE 7 or later.
  
  
 ## Installation
 ### Build
 Run command-line in the project path and call it on command-line.
  ```sh
  mvn clean install
  ```
  
  ### Run
  
  Run **MongoDB** and go to [http://localhost:8080/crawler/{twitterUser}](http://localhost:8080/crawler/{twitterUser})

Call these commands for running test classes.

```sh
mvn test
```
or one
```sh
mvn -Dtest=CrawlerControllerTest  test
mvn -Dtest=CrawlerServiceTest  test
mvn -Dtest=FriendShipCrudServiceTest  test
mvn -Dtest=FriendShipScoringServiceTest  test
mvn -Dtest=FriendShipServiceTest  test
```
