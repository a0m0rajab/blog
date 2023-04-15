+++
author = "Abdurrahman Rajab"
title = "Resetting PostgreSQL password"
description = "Password resetting tips for PostgreSQL"
date = "2023-04-16"
tags = [
    "Learning",
    "Linux",
    "sysadmin",
]
categories = [
    "Learning",
    "Linux",
    "sysadmin",
]
aliases = ["PostgreSQL_tips"]
+++

Forgetting a password is one of the most painful things you can have or can happen! but it's always a way to learn new tools and solutions.

Here is a solution in case if you forgot your PostgreSQL password:

1. Locate the pg_hba.conf file
   1. in windows it's under ```C:\Program Files\PostgreSQL\12\data```
2. edit the conf file
   1. change the connection to trust. in the method area. 
3. restart Postgres service
   1. from service or  by using ```pg_ctl -D "C:\Program Files\PostgreSQL\12\data" restart```
4. set the password
   1. ```postgres=# ALTER USER postgres WITH PASSWORD 'new_password';```
   2. you can use this in the password area
5. restore the conf file.
   1. change the information back to the previous situation

Helpful resources:

- [Postgre Sql tutorial](https://www.postgresqltutorial.com/postgresql-administration/postgresql-reset-password/)
 