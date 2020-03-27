Once you've made sure you have Docker installed. You should make sure that all prerequisits are installed. 

First: Docker Compose has to bee installed. This is a Docker tool for running multi-conntainer Docker packages (such as BuildBot).
You can do this by running `pip install docker-compose`{{execute HOST1}}

Second: You want to make sure that Docker will work fine. This can be done by running the command `sudo docker run -i busybox /bin/echo Success`{{execute HOST1}}
This command will download BusyBox if not available and try to print the message "Success". If "Success" is printed, your installation of Docker is ready for the BuildBot image.