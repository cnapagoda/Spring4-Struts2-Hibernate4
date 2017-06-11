# Spring4-Struts2-Hibernate4
Spring4, Struts2 and Hibernate4 based sample web project

In this sample project , I have integrated Structs2 and Spring 4 with Hibernate 4 using annotation based configuration. This project includes a simple CRUD java application, creating hibernate entities, saving data in MySQL database , performing database CRUD operations within transaction using annotation based configuration. 

How to Run this project

- Create a database called `chandana`
- Compile the project using maven:
    ```sh
    $ mvn clean install
    ```
- Run using jetty plugin
    ```sh
    $ mvn jetty:run
    ```
- Access the `http://localhost:8080/Spring4/`



### Struts 2 - Interceptors

Struts2 Interceptors are responsible for most of the processing inside the Struts2 framework. You can register interceptor in Action class level or default for all action.


    
    @InterceptorRef(value="customStack")
    
or
    
    <default-interceptor-ref name="customStack"></default-interceptor-ref>
    


### Struts 2 - different ways to create Action classes

- Implementing Action interface
- Using Struts2 @Action annotation
- Extending ActionSupport class(Ex: LoginAction -  I used this option. There you can override methods validate and execute methods.)


### Structs2 - Validation support.

The Struts validation framework provides inbuilt validation support. In this sample I have implemented required string validation, so please refer LoginAction class. 
