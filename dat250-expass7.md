# Lab 7 - Pub/Sub pattern with RabbitMQ and AMQP 

## Experiment 1

Installed and ran RabbitMQ with the docker using the command  
`docker run -it --rm --name rabbitmq -p 5672:5672 -p 15672:15672 rabbitmq:3.9-management` 
given in the [download section](https://www.rabbitmq.com/download.html) from RabbitMQ website. 

## Experiment 2 and 3

Was done as described. 
The writing of the logs to the disk did not work, probably because of using powershell and not BASH as they seem to expect. Did not try to fix this as this seems really trivial and everything else worked as expected.

The code for this assignment can be found [here](https://github.com/mrtineide/expass7)