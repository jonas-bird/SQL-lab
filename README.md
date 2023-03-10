# SQL lab scripts 

## Initial setup 

In order to simplify learning SQL and not need to mess around with my system's version of PostgreSQL I am going to use the [official Docker image](https://www.docker.com/blog/how-to-use-the-postgres-docker-official-image/)  

I don't plan on needing to access the data from other applications so I am going to let Docker manage the files.  

So: 
``` sh
docker run -d \
    --name postgres-tut \
    -p 5432:5432  \
    -e POSTGRES_PASSWORD=cstutorials  \
    -v postgres:/var/lib/postgresql/data  \
    postgres

```
I am not sure which GUI I am going to settle on so I may end up trying a few different ones. 
