# Spring MVC 4 + Spring Security 4 + Hibernate Example

A sample demonstration of Spring MVC with Hibernate

# Pre Requisites
- Latest Version of Java (Used version is 1.8.0_171)
- Tomcat 8 (Used version is 8.5.30)
- MySQL Server 5.7 ( Used version is 5.7.22)
- Maven (Used version is 3.5.2)
- Git
- Latest version of eclipse of you need to playaround with the code

# Environment Preparation
Follow the below stpes 
  - Install Java and set the JAVA_HOME environment variable to the installed java directory ( For Exmaple /usr/lib/jvm/java-8-oracle
  - Install Tomcat 8
  - Install the mysql server
  - Install Maven
  - Install Git

# Database preparation

Execute the SpringMVCHibernateWithSpringSecurityExample/db.sql after connecting to mysql as root user

# Build

- Clone this repository
- switch to SpringMVCHibernateWithSpringSecurityExample and run the mvn command
```sh
$ cd SpringMVCHibernateWithSpringSecurityExample
$ mvn clean install
```
# Deployment
- The ablove command will generate the war file SpringMVCHibernateWithSpringSecurityExample.war under SpringMVCHibernateWithSpringSecurityExample/target directory
- Put this war file into tomcat webapps folder
- Restart the tomact server

# Usage

In a browser access the application using the below URL
```sh
$ http://localhost:8080/SpringMVCHibernateWithSpringSecurityExample/
```
- Login with User 'Sam' & password 'abc125'
# Summary
The project shows a simple user-management application. One can create a new user, edit or delete an existing user, and list all the users. User can be associated with one or more UserProfile, showing many-to-many relationship. URL’s of the applications are secured using Spring Security. That means, based on the roles of logged in user, access to certain URL’s will be granted or prohibited. On the view layer, user will see only the content he/she is allowed to based on the roles assigned to him/her, thanks to Spring Security tags for view layer.
