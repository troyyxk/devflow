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
## Data
```
Companies:
	{
        "members": list of members in the company :list,
        "teams": list of team in the company :list,
        "_id": the id of the company :string,
        "name": name of the company" :string,
        "bossId": id of the boss :string,
        "companyPic": url :string
        }
Teams:
	{
        "members": list of members in the team :list,
        "tasks": list of tasks in the team :list,
        "_id": id of the team :string,
        "companyId": id of the company :string,
        "teamName": name of the team :string,
        "leader": id of the team leader :string,
        "quote": team quote :string,
        "teamPic": team profile picture :string,
    },
	Tasks:
		    {
        "_id": the id of the task :string,
        "companyId": the id of the company :string,
        "name": name of the task :string,
        "estimatedTime": estimated time of the task :string,
        "usedTime": time been used of the task :string,
        "teamId": the id of the team :string,
        "assignedToId": the member id of assign the task by :string,
        "assignedById": the member id that assign the task to :string,
        "taskDetail": task details :string,
    },
Members:{
        "rank": the rank of the member :string,
        "teamId": the team Id of the member :string,
        "profilePic": the profile picture of the member :string
 "isApproved": member approval in the company :string,
        "_id": the id of the member :string,
        "firstName": member’s first name :string,
        "lastName": member’s last name :string,
        "userName": member’s login username:string,
        "companyId": member’s company Id :string,
        "password": member’s password :string,
    },

	Notification:
       {
        "from": the sender’s member id :string,
        "isUnread": check if notification is unread :string,
        "_id": the id of the notification :string,
        "level": the level of the notification(1:personal,2:team...so on) :string,
        "to": the receiver’s member id :string,
        "message": the content/message of the notification :string,
        "time": the time sent of the notification(2020-03-17T22:15:00.000Z) :string,
    },


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
