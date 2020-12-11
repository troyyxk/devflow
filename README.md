# Devflow

To start the project follow the following instructions:
```
npm run build
```

After that,  run:
```
npm run start
```

You will be at the intro page.

Navigate to the loggin page, loggin with:
```
Username: user
Password: user
```
Then you will login as admin

Navigate to the loggin page, loggin with:
```
Username: admin
Password: admin
```
Then you will login as admin

To check other users, please take a look at our data base at
```
mongodb+srv://team34:team34Password@devflow.oddf0.mongodb.net/devflow
```

## Routing table:

### auth.js
```
/login
requset type: post
sample request body: 
{ "data": { "userName": "user", "password": "user" } }
result: the login user data


```
