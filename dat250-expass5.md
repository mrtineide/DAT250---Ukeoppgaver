# Lab 5 - Springboot 

Code for each assignment can be found under the [expass5](https://github.com/mrtineide/expass5) repo. In that repo there is a submodule for each experiment. 

## Experiment 1 - Springboot quickstart
Code for the assignment can be found [here](https://github.com/mrtineide/springbootdemo_dat250) or under the submodule springbootdemo_dat250 in the [expass5](https://github.com/mrtineide/expass5) repo.

## Experiment 2 - Building an Application with Spring Boot
Trying to run the ``spring-booot:run`` with the ``mvnw`` did not succeed. The error given was
```
Error: JAVA_HOME not found in your environment.
Please set the JAVA_HOME variable in your environment to match the
location of your Java installation.
``` 
Instead, by using the already installed mvn command/program the expected output was given and spring-boot was loaded. 
There were a lot of new words end terminology that was not previously know. Such as:
- WAR file deployments
- Tomcat
- "Is * on the classpath"
- what inserting a bean in the context of spring

The "JAR Support and Groovy Support" step in the tutorial was skipped.

There were many compnents to this application that were not explained the need for and the impression was that 
a lot of not really needed components added to the application. 
The activity of tutorial consisted of copy and pasting, and just reading outputs and text. 
Overall the perceived knowledge gained from this tutorial was small.  

Code can be found [here](https://github.com/mrtineide/gs-spring-boot) 

## Experiment 3 - Building a RESTful Web Service

The tutorial mentions:

_This application uses the Jackson JSON library to automatically marshal instances of type Greeting into JSON. Jackson is included by default by the web starter._

Where does this come from? How does this happen?
How it does this is not transparent to the developer from the source code. 
It says that the Jakson2 library that handles JSON translation is on the classpath. But what does that mean in this context?

Rest of the experiment was done as described. 

Code can be found [here](https://github.com/mrtineide/gs-rest-service)

## Experiment 4 -Accessing Data with JPA

The experiment was an exercise that was easier to see why it is needed and how it works, unlike the other experiments.

Code can be found [here](https://github.com/mrtineide/gs-accessing-data-jpa)