# Basic Keycloak example with two different applications

## Requirements:

* docker and docker-compose
* node >= 8 + npm
* add to /etc/hosts the following lines:

```
127.0.0.1 app1 app2 keycloak 
```

Open the browser at http://keycloak:8080/ and login with username: 'admin', and password: 'admin'.

Open the Keycloak admin console, click on Add Realm, click on import 'Select file', select nodejs-example-realm.json and click Create.

## Basic setup

Install the dependencies and start NodeJS example by running:

```
$ cd app1 && npm install
$ cd app2 && npm install
```

Open the browser at http://app1:3000/
Open the browser at http://app2:4000/


## Running the playground

```
$ docker-compose up
```



