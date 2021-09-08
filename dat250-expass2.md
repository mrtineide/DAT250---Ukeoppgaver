
# Lab 2
## Experiment 1 - Application using JPA

Did not understand wat was meant in the todo in the persistance.xml so asked for help on the (digital) lab session and figured out what was meant by the todo. Was succsesfull in verifying the installation afterwards. 

Step 5 in the tutorial mentions that we use lombok for simplifying the data object code, by auto-generationg getters and setters. Tried to copy paste the provided code but IntelliJ marked the lombok package as missing.
Tried to add it as a dependency in the pom.xml but alas no result.
Tried to add the pom.xml snippet provided at https://mvnrepository.com/artifact/org.projectlombok/lombok/1.18.12 but no better result either. 
''' xml
<!-- https://mvnrepository.com/artifact/org.projectlombok/lombok -->
<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok</artifactId>
    <version>1.18.12</version>
    <scope>provided</scope>
</dependency>
'''

In the depenencies tab in IntelliJ the lombok package is not present. Suspect this means that maven has not downloaded the jar.
Tried to run 'mvn clean install' with the hope that the dependencies would be reloaded.
Searched on Google with "dependency red in intellj" and one of the suggestions said to restart intellij. This fixed the issue. 
This could probably been solved a different way. One possible root problem is that IntellJ uses a maven that is bundeled with and not the seperate installed maven from last lab. Not sure if this is the case though.  
Then found out it by [this blogpost](https://stackoverflow.com/questions/9980869/force-intellij-idea-to-reread-all-maven-dependencies) that it was possible by ctr+shift+a to bring up the actions menu and use the action "Reload all Maven Projects". Can not veify that this would have worked as the issue is fixed prior to finding this. But on another student did this and it verifiably fixed the issue

On step 6 in the tutorial 2 hours were spent trying to follow the tutorial step of making a new project. The project structure was incorrect for every iteration that was tried. 
The fix was to not follow the tutorial but instead just edit the persistance.xml iterativly until the Unit test were green.

Inspecting and connectig the database was done using this [tutorial] (https://www.jetbrains.com/help/datagrip/apache-derby.html) with Datagrip, the database IDE from Jetbrains.
This could also be done in IntelliJ from the databases tab.

Getting some diagrams was done following using [this](https://www.jetbrains.com/help/datagrip/creating-diagrams.html)

Here is an example of a table made:

![Table example](/db_tables_example.png)


Here is a diagram of the tables made:

![Diagram of tables made](/db_tables.png)


