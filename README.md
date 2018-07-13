#Basic NodeJS Example
* need to upgrade to use hapi 17


##Start and configure Keycloak

###Start Keycloak:

```
/<Path-To-Keycloak>/bin/standalone.sh
```

Open the Keycloak admin console, click on Add Realm, click on import 'Select file',
select nodejs-example-realm.json and click Create.

Link the HEAD code of keycloak-hapi by running:

```
npm link ../
```

Install the dependencies and start NodeJS example by running:

```
npm install
npm start
```

Open the browser at http://localhost:3000/ and login with username: 'user', and password: 'password'.

# TODO
* sometime you may get "ERR_TOO_MANY_REDIRECTS", need browser to clean cookie before normal
