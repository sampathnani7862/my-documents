# my-documents
my documents 
https://tecadmin.net/how-to-install-mysql-8-on-amazon-linux-2/  ---------->mysql-8-on-amazon-linux-2/
https://www.jenkins.io/doc/tutorials/tutorial-for-installing-jenkins-on-AWS/ ------------->jenkins
container  is the concept next to virtual machine ,it is nothing but the imlimentation of VM.
to run any application the main importent is it should have mainly libraries and binaries 
in containerization we mainly concentrate on minimal os ,more on application  
each container is isolated with each other and used resources from host os of how much t requir not a specific value
in docker it have mainly docker engine,docker demoen,docker host,docker server all these act as a host operating system.and container will act as a guest operating system.
https://labs.play-with-docker.com/ -------> is used for docker play ground terminal it has all library and dependency which are required.before logging into it you must have to log in to docker hub with your own account.
#   $ curl -fsSL https://get.docker.com -o get-docker.sh     ---->    #   $ sh get-docker.sh   ---------> https://get.docker.com/
  docker is light weight,migration is very easy of any application  
we can maintain two different versions of softwares in a containerization like tomcat 8 tomcat9 in the isolated containers.
to login to docker we have different ways they are aws console,docker play ground .
launch any instace with any os like ubuntu, amazon ec2,rethat,centos etc.
#[ec2-user@ip-172-31-61-205 ~]$ whoami    ----> to check the which os you have used for launching the instance
ec2-user  
#[ec2-user@ip-172-31-61-205 ~]$ sudo -i  -----> change to root account from sudo   $---> indicates sudo user (super user)
#[root@ip-172-31-61-205 ~]#sudo apt update    --->fot ubuntu       #----> indicates root user
#sudo yum update ---> for amazon ec2
#sudo yum install docker  ---> to install the latest version of docker 
#docker -v      or     docker --version      or docker version
#docker info
#sudo systemctl start docker 
#sudo systemctl restart docker 
#sudo systemctl status docker
cd ~
    
    8  sudo usermod -aG docker ec2-user  ----> to give docker permission as a user
   12   exit
   13  docker info
   14  init 0
   15  apt update
   16  sudo yum update
   17  ls
   18  ls -la
   19  sudo yum install docker
   20  docker info
   21  dockeer -v
   22  docker -v
   23  sudo usermod -aG docker ec2-user
   24  sudo system start docker
   25  docker -v
   26  docker info
   27  sudo systemctl start docker
   28  sudo systemctl restart docker
   29  sudo systemctl status docker
   30  docker info
   31  whoiam i
   32  whoami
   33  cd ~
   34  exit
   35  docker info
   36  sudo chmod 666 /var/lib/docker
   37  docker info
   38  sudo chmod 666 /var/run/docker.sock
   39  docker info
   40  docker version
   41  id
   42  cd ~
   43  exit
   44  docker --help
   45  docker ls
   46  sudo docker ls
   47  docker container ls
   48  docker run hello-world
   49  docker ps -a
   50  docker ps
   51  docker pull hello-world
   52  docker pull nginx
   53  docker images ls
   54  docker image ls
   55  docker run -d httpd      ----> to make the container in the detached mode so that it cannot get excited 
   56  docker image is
   57  docker image ls
   58  docker container ls
   59  docker ps -a
   60  docker run -d sampath
   61  docker image ls
   62  docker ps
   63  docker container run ubuntu sleep 20
   64  docker ps -a
   65  docker container httpd stop
   66  docker ps -a
   67  docker stop 0f0d6ff2af66
   68  docker ps -a
   69  docker restart 0f0d6ff2af66
   70  docker ps -a
   71  docker container run -it httpd /bin/bash
   72  docker ps -a
   73  exit
   74  docker ps -a.
   
   Docker i swritten in GO language Go language include all the commands also
   OS patching security level it is good in containers 
   ------------------------------------------------------------------------------------------------------------------------------------------------------
   Docker commands
   the topics in docker is as follows
   1.docker file
   2.docker compose
   3.docker storage
 
 #docker info ---> if it shows the error then run the following commands first start the docker #sudo systemctl start docker     #sudo systemctl status docker 
 then run the #docker info    ----> you will not gwt any error.
 #sudo systemctl enable docker ----> when we stop that perticular instance and start after some time or day later 
 we need to start the docker again but if we give the above command their is no need of starting the docker again when the instace starts the docker automatically start update
#sudo systemctl enable docker  ---->part of init.d   --->enable is not only for docker it also for jenkins and others also.
the server start automatically.
docker hub:-it is a centralized server where all the images are placed and it is a public repository
ctrlp+ctrlq --------> if u execute the command docher run -it ubutu /bin/bash
root ---> but you want to run exit command to come out, then press  ctrlp+ctrlq 
docker stop $(docker ps -aq)    ------------->to stop all containers
 docker rm $(docker ps -aq)
 docker ps --filter status=running
 docker stop $(docker ps --filter status=running -q) 
 docker rm $(docker ps --filter status=exited -q)
 docker rm $(docker ps --filter status=exited -q)
 1  cd ~
    2  sudo yum update
    3  sudo apt install
    4  yum apt install
    5  yum apt update
    6  sudo -i
    7  docker -v
    8  sudo usermod -aG docker ec2-user
    9  sudo systemctl start docker
   10  sudo systemctl status docker
   11  docker info
   12   exit
   13  docker info
   14  init 0
   15  apt update
   16  sudo yum update
   17  ls
   18  ls -la
   19  sudo yum install docker
   20  docker info
   21  dockeer -v
   22  docker -v
   23  sudo usermod -aG docker ec2-user
   24  sudo system start docker
   25  docker -v
   26  docker info
   27  sudo systemctl start docker
   28  sudo systemctl restart docker
   29  sudo systemctl status docker
   30  docker info
   31  whoiam i
   32  whoami
   33  cd ~
   34  exit
   35  docker info
   36  sudo chmod 666 /var/lib/docker
   37  docker info
   38  sudo chmod 666 /var/run/docker.sock
   39  docker info
   40  docker version
   41  id
   42  cd ~
   43  exit
   44  docker --help
   45  docker ls
   46  sudo docker ls
   47  docker container ls
   48  docker run hello-world
   49  docker ps -a
   50  docker ps
   51  docker pull hello-world
   52  docker pull nginx
   53  docker images ls
   54  docker image ls
   55  docker run -d httpd
   56  docker image is
   57  docker image ls
   58  docker container ls
   59  docker ps -a
   60  docker run -d sampath
   61  docker image ls
   62  docker ps
   63  docker container run ubuntu sleep 20
   64  docker ps -a
   65  docker container httpd stop
   66  docker ps -a
   67  docker stop 0f0d6ff2af66
   68  docker ps -a
   69  docker restart 0f0d6ff2af66
   70  docker ps -a
   71  docker container run -it httpd /bin/bash
   72  docker ps -a
   73  exit
   74  docker ps -a
   75  exit
   76  history
   77  exit
   78  sudo -i
   79  history
   80  docker ps -a
   81  df -h
   82  ip -a
   83  config ip
   84  history
   85  sudo chmod 666 ///var/run/docker.sock
   86  sudo chmod 777 /var/run/docker.sock
   87  cd ~
   88  exit
   89  docker info
   90  sudo chmod 666 /var/run/docker.sock
   91  sudo -i
   92  exit
   93  docker --version
   94  docker version
   95  sudo systemctl start docker
   96  sudo systemctl status docker
   97  docker info
   98  sudo systemctl enable docker
   99  sudo systemctl status docker
  100  docker -H
  101  docker ps -a
  102  docker image ls
  103  docker container run alpine
  104  docker image ls
  105  docker ps run -d alpine
  106  docker container run -d alpine
  107  docker ps
  108  docker ps -a
  109  docker run -d alpine
  110  docker ps
  111  docker ps -a
  112  docker run -d httpd
  113  docker ps -a
  114  docker ps
  115  docker run -d ubuntu
  116  docker ps
  117  docker ps -a
  118  docker start 49c7cc9a1951
  119  docker ps
  120  docker container run -it alpine /bin/sh
  121  docker ps
  122  docker container run -it ubuntu
  123  dosker ps
  124  docker ps
  125  docker ps -
  126  docker ps -a
  127  docker stop f7d562ad921c
  128  docker ps -a
  129  docker start f7d562ad921c
  130  docker ps -a
  131  history

 



 
