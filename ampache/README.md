# ampache-docker

Basic setup for Ampache with docker-compose with persistant configuration and mysql data.

Notes:

 1. The ./conf/ampache and ./mysql directories need to be empty as the container will copy data into them the first time your run it.
 1. The ./conf/ampache and ./mysql directories also need to be writable by the processes inside the docker container.  The easiest way to figure this out is to use "chmod 777 ./conf/ampache ./mysql" before running "docker-compose up" for the first time.  After you've run the docker the first time look at the ownershop of the files within the directories and lock down ./conf/ampache and ./mysql appropriately.
 1. The DAAP setup isn't working for me yet and I haven't had a chance to figure out why.
