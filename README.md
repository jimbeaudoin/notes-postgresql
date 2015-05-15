# notes-postgresql
PostgreSQL notes for myself.

## Installation (Ubuntu 14.04)
Create the file /etc/apt/sources.list.d/pgdg.list
```sh
deb http://apt.postgresql.org/pub/repos/apt/ trusty-pgdg main
```
Import the repository signing key, and update the package lists
```sh
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | \
  sudo apt-key add -
sudo apt-get update
```
Install PostgreSQL
```sh
sudo apt-get install postgresql-9.4
```
Install lib
```sh
sudo apt-get install libpq-dev
```

User Creation
```sh
sudo su - postgres
createuser -d <username>; # -d Allowed to create databases
```
Database Administration
```sh
sudo su - postgres
psql
```
