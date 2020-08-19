Here is all postgres data from /var/lib/postgresql/data.
One issue: over using docker-compose build and docker-compose up -d
I've got changes in postgres-data permissions from 755 to
drwxrwxr-x 20 systemd-coredump gregory 4096 авг 19 08:29 postgres-data
So to wath and edit this dir:
sudo chmod 775 postgres-data
in ${dockerProjectName} root