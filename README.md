# :closed_book: General info:
Hello! This is my first web-api, where I used the knowledge in Java Core, OOP and SOLID principles, JDBC and WEB.

# :oncoming_taxi: About project:
This is simple taxi service, where we first need to register or authenticate and after we can:

- Add/Delete/ShowAll driver :man_pilot:
- Add/Delete/ShowAll manufacturer :factory:
- Add/Delete/ShowAll car :car:
- Add driver to car :taxi:

# :abacus: Technologies used:

- Java 11
- JDBC
- Java Servlets
- MySQL
- Apache Tomcat 9.0.50
- Log4j2

# :computer: If you want to run this project, you need:
1. to have or install MySQL and Apache Tomcat 9.0.50
2. clone this project
3. create DB schema and tables using `init_db.sql` file from `resources` directory
4. add your credentials to ConnectionUtil located in util to connect to your database
```java
public class ConnectionUtil {
    private static final String URL = "YOUR CONNECTION URL";
    private static final String USERNAME = "YOUR LOGIN";
    private static final String PASSWORD = "YOUR PASSWORD";
    private static final String JDBC_DRIVER = "JDBC DRIVER";
}
```
6. add Tomcat configuration to your project. Use `/` as your Tomcat application context
7. configure `log4j2.xml` from `resources` directory. Add correct path to the `app.log` file

After all these steps you will be able to run this project locally.

## :globe_with_meridians: Or you can test this project online: https://taxi-servicesss.herokuapp.com/login