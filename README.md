# Weather-Search-Panel-With-History---Openweather-API-JQuery-NodeJS-MySQL

A basic implementation of a meteorological survey panel, with data from the OpenWeathermap API, this datas was captured in JSON through AJAX. Implementation of the server in NodeJS connected to MySQL, implementation of the client in JQuery.

# Configuration

To run this code it is necessary to install the NodeJS library, download here: https://nodejs.org/en/download/

It is also necessary in this project to install the MySQL server, for which I recommend using the Laragon App: https://laragon.org/download/index.html.

The implementation includes module bellow:
```
*const express = require('express');
*const path = require('path');
*const bodyParser = require('body-parser');
*const mysql = require('mysql');
*const fs = require('fs');

```
If you do not have the following module, you will need to perform the installation using the commands.

To install the necessary module just follow the steps below, in NodeJS terminal:

```
# Install express module
$ npm install express

# Install path module
$ npm install path

# Install body-parser module
$ npm install body-parser

# Install mysql module
$ npm install mysql

# Install fs module
$ npm install fs
```

# Mysql Database

Here at the root of the project is a file containing the table implemented to record the history. With name "BD_mySQL.sql".

Before uploading the table, it is necessary to create the database with the name "testenode". To do so, simply run the following MySQL commands:

```
CREATE DATABASE testenode;
```

To upload the table, just run in the terminal:

```
mysql -u username -p testenode < BD_mySQL.sql
```

To change bank settings, such as login, flock name, etc. Just change the following excerpt in the "server.js" file:

```
var con = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "root",
  database: "testenode"
});
```

# How to Use

To run the app, just start the virtual server in the NodeJS terminal, as shown below:

```
node server.js
``` 

Depois basta acessar o servidor local pelo navegador através da porta configurada: http://localhost:8080/


# Demonstration

Next, a video shows the final result of the implementation:

https://youtu.be/hgtNn7QBDiY
