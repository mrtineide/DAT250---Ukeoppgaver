

In particular, you should write about:

    technical problems that you encountered during installation of the software development environment and how you have solved them
    how you have validated (checked) that the software development environment is working
    technical problems encountered with the Heroku platform and how you solved them
    any pending issues with this assignment which you did not manage to solve

## Lab 1 - Installing java, maven, IDE and a git client

Already have git and github client installed. I know this works as I used both clients to make this repo and push my changes
I choose to install IntelliJ IDEA as the IDE. In conjunction I made suke i hade a JDK installed as requierd by Maven. I used a INF112 project and ran it to validate both IDE and Java JDK.
Maven was installed and added to PATH env and validated with the command "mvn -v" as per the install instructions.  

## Heroku - deploy a java app

Problem: Heroku run java -version
The connection timed out.
May be firewall blocked the port 5000 for incoming traffic so can not connect the proccess to the terminal. So far have not done anything to fix it. Running Wireshark we can see in a ICMP message from the default gateway adress that the "destination unreachable" because of "communication adminastrative filtered". 
At some point in the heroku tutorial we are asked to make a permanent log with that requiers to add a credit card to verify the account. This is also needed to add a database. So I skipped this step. 