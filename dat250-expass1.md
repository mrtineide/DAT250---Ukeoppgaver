
# Lab 1
## - Installing java, maven, IDE and a git client

Already have git and github client installed. Validation of it working was done by using both clients to make this repo and push the changes made. 
Choose to install IntelliJ IDEA as the IDE. In conjunction it was made sure that the computer had a JDK installed as required by Maven. A INF112 project was used to  validate both IDE and Java JDK. It worked as expected.
Maven was installed and added to PATH .env and validated with the command "mvn -v" as described in the maven install instructions.  

## Heroku - deploy a java app

Almost everything went smoothly, followed the tutorial as is. The one thing there was a problem with was this command here: `heroku run java -version`
The connection timed out.
May be a firewall blocked the port 5000 for incoming traffic so can not connect the process to the terminal. Running Wireshark we can see in a ICMP message from the default gateway address that the "destination unreachable" is the reason, because of "communication administrative  filtered". So the solution was  to use a different network, which did resolve the issue. Changed from HVL provided Eduroam to a UiB provided Eduroam.
At some point in the heroku tutorial we are asked to make a permanent log with that requires to add a credit card to verify the account. Skipped this step because of this.

[Link to Heroku java site](https://damp-brushlands-26239.herokuapp.com/)

### Remarks
Did not feel that I learned that much about the frameworks used and hopefully we are to learn more about them in the future. But the goal of the exercise was fulfilled.