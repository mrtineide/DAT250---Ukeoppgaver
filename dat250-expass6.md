## Lab 6 - Front-end technologies

## Experiment 1 - MVC web app

Everthing was done as described in the tutorial. 

The code for this experiment can be found [here](https://github.com/mrtineide/gs-serving-web-content)

## Experiment 2 - Single Page Web Application

The hot reload did not work. According to [this blogpost](https://mbuotidem.github.io/blog/2021/01/09/how-to-hot-reload-auto-refresh-react-app-on-WSL.html) the root cause for this issue is that node and npm is running on WSL2 but the project is saved on the Windows files system and therefore the hot reload does not work.

The code for this experiment can be found [here](https://github.com/mrtineide/react-tut-dat250)