* BEFORE  ALL

you should submit you have a clean install, no pervious docker volume left!

 ************
 1. be sure that variable "debug" in **./ckan/config/deployment.init_tmpl** be true .

 2. in **./contrib/docker/docker-compose.yml** to open step1 and comment code for step2 && rename the **.env.template** in the same path to **.env**

 3. run command  **docker-compose up -d --build** in path **./contrib/docker/**

 4. use command **docker cp** to copy out of conatianer "ckan"(/etc/ckan, usr/lib/ckan, /var/lib/ckan) && down the compose 

 5. in **./contrib/docker/docker-compose.yml** to open step2 and comment code for step1

 6. change the **CKAN_DEV_LOCALTION** for you pervious copy in **.env** 

6. run command **docker-compose up -d --build** again

7. done