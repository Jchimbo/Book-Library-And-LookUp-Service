# Book Library And LookUp Service
A simple backend and frontend for  storing a booklist and searching for books using springboot and Google Oauth.

## Requirements

### MySQL
Please use this guide to setup [MYSQL](https://www.digitalocean.com/community/tutorials/how-to-install-mysql-on-ubuntu-22-04).

This project requires a MySQL database to be up and running the database's
information can be customized in the application properties file located in /src/main/java/resources.

The database is structured so that there are two required tables users, and book_list. 

The users table is made up of two columns
user_name and user_email, where the primary key is user_name. 

The book_list table is made up of two columns, user_name and book_ibsn, where the primary key is a composition of both columns.

### GOOGLE OAUTH
Please follow these steps to get a client_id, client_secret, and a token_uri, [GOOGLE OAUTH](https://developers.google.com/identity/protocols/oauth2).

### GOOGLE BOOKS API
You will also need a google api key to access the google book api. This is to serve as the api that will handle request from the frontend of the application.
Click on credentials link to get an API KEY from the [BOOKS API](https://developers.google.com/books/docs/v1/using#APIKey).
