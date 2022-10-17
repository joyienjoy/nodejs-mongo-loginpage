# nodejs-mongo-loginpage
A simple User Registration and Login Page


Target:
A Login Page is Created
A User can Register - first time. Data is stored in MongoDB
A user can Login - Using registed credentials - On Login, Your details will be shown on output.

View at MACHINE-IP:3000  
![image](https://user-images.githubusercontent.com/92083624/195572231-2dca0572-9cdb-4e28-97ff-1b4cfc764909.png)


View at MACHINE-IP:3000/login
![image](https://user-images.githubusercontent.com/92083624/195572546-57811000-dd70-4ea6-90aa-10d3528c19a8.png)

View at MACHINE-IP:3000/forget-pass
![image](https://user-images.githubusercontent.com/92083624/195572749-bc63dfba-92f9-41e1-a2ca-7fc9724c022f.png)

If you use
mongosh    #To see inside database
use ManualAuth    #The database created by the application for saving user data
show collections   # To see various data collections saved by application. You will see collection named "users"
db.users.find().pretty()  # To see contents of all registed users

![image](https://user-images.githubusercontent.com/92083624/195573679-daa26afd-eb0d-47fb-ad47-50dbed234811.png)


Essentials of Docker Compose 
1. The name of the MONGODB container is used in the URL of database in server.js to use mongoose.connect
2. Volume mounting is done to avoid losing data
