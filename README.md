# react-spring-integration
Integratie the react.js frontend and spring boot backend

# 1.) Backend - Spring Boot App Setting 

Create Spring Boot App by using Eclipse or Sprint Tool Suit

pom.xml (Default)
![alt text](https://user-images.githubusercontent.com/9346306/54796240-60846d00-4c8a-11e9-82bb-4806cd7dcf24.jpeg)

Add a TestController for connection test
￼
![alt text](https://user-images.githubusercontent.com/9346306/54796245-61b59a00-4c8a-11e9-9b4e-6da3c047b092.jpeg)


Add a folder named “public” under spring-boot-backend/target/classes/
(This folder is for store react-frontend)
![alt text](https://user-images.githubusercontent.com/9346306/54796231-5ebaa980-4c8a-11e9-97dd-413049ca1ea0.jpeg)


## Run the application, spring boot backend is ready!!!!


# 2.) Frontend - React Web Setting

Create React App by running below cmd:
```
npx create-react-app react-frontend
cd react-frontend
npm start
```
![alt text](https://user-images.githubusercontent.com/9346306/54796237-60846d00-4c8a-11e9-991f-00e26e5d03a5.jpeg)

Now you will able to see the react js fontend.

Stop the services by press Ctrl + C

Update react-frontend/package.json setting. Add proxy setting point to your sprint-boot-backend.
![alt text](https://user-images.githubusercontent.com/9346306/54796239-60846d00-4c8a-11e9-8434-772b03a5f0c5.jpeg)


Update react-frontend/src/App.js for testing the connection.
![alt text](https://user-images.githubusercontent.com/9346306/54796232-5f534000-4c8a-11e9-940e-8b11723e2f9c.jpeg)

Run below cmd (Make sure your spring-boot-backend is up and running) otherwise, you will can error.

```
npm start 
```


![alt text](https://user-images.githubusercontent.com/9346306/54796243-611d0380-4c8a-11e9-85f0-b7c6d7fc0070.jpeg)
￼￼

(If you hit this error, you need to make sure your spring boot backend is up and running)

![alt text](https://user-images.githubusercontent.com/9346306/54796244-61b59a00-4c8a-11e9-80ff-30ea8ec8ff07.jpeg)
￼￼

(Success to connect spring)

Stop the services by press Ctrl + C

Run below cmd to build react project 

```
npm run build
```

Check the react-frontend folder structure that contain build folder
![alt text](https://user-images.githubusercontent.com/9346306/54796241-611d0380-4c8a-11e9-989d-3fa36d372883.jpeg)

## React web is ready!!!!

# 3.) Integrate two projects

Copy all the files/folders inside react-frontend/build to spring-boot-backend/target/classes/public. Final struct like below.

![alt text](https://user-images.githubusercontent.com/9346306/54796234-5febd680-4c8a-11e9-91da-4065ac357f21.jpeg)

Restart the spring-boot-backend App. 

![alt text](https://user-images.githubusercontent.com/9346306/54796233-5f534000-4c8a-11e9-8b51-2ce7c9d9911f.jpeg)

React is already intergrated with spring!!!! Running at port 8080

Done

