# The backend part of the qr-project app

## Layers Structure:

Basically: CRUD, checking info, inventory pre and post process handling, authorization,
docs and file converting, qr-image creation.

rest - RestApi - api to handle requests
model - pojo
dao - additional pre db or post db action later to change the object
mapper - Mybatis - db connection and sql queries

additional -
    JsonHandler for data storing in db
    SqlBuilder - build a complex query from the list of objects (cause we use annotations)
    Utility - parsing xml in different ways (one column, a lot etc)

config - Corsfilter - allow to call the api from different sources
    CustomUserDetailService - authorization with user name and role check
    WebSecurityConfig - who, with which role can go, passw encoder, authentification
test - several examples of the tests (unit and integration)

