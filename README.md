# react-spring-integration
Integratie the react.js frontend and spring boot backend

# 1.) Backend - Spring Boot App Setting 

Create Spring Boot App by using Eclipse or Sprint Tool Suit

pom.xml (Default)
￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/pom.xml.jpg)

Add a TestController for connection test
￼
![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/testController.jpg)


Add a folder named “public” under spring-boot-backend/target/classes/
(This folder is for store react-frontend)
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/add%20public%20folder.jpg)


## Run the application, spring boot backend is ready!!!!


# 2.) Frontend - React Web Setting

Create React App by running below cmd:
```
npx create-react-app react-frontend
cd react-frontend
npm start
```
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/npm%20start.jpg)

Now you will able to see the react js fontend.

Stop the services by press Ctrl + C

Update react-frontend/package.json setting. Add proxy setting point to your sprint-boot-backend.
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/package%20json.jpg)


Update react-frontend/src/App.js for testing the connection.
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/call%20to%20testController.jpg)

Run below cmd (Make sure your spring-boot-backend is up and running) otherwise, you will can error.

```
npm start 
```


￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/react%20fail.jpg)
￼￼

(If you hit this error, you need to make sure your spring boot backend is up and running)

![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/react%20success.jpg)
￼￼

(Success to connect spring)

Stop the services by press Ctrl + C

Run below cmd to build react project 

```
npm run build
```

Check the react-frontend folder structure that contain build folder
![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/react%20build%20folder.jpg)

## React web is ready!!!!

# 3.) Integrate two projects

Copy all the files/folders inside react-frontend/build to spring-boot-backend/target/classes/public. Final struct like below.

![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/integrated%20spring%20and%20react.jpg)

Restart the spring-boot-backend App. 

￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/final%20resutl.jpg)

React is already intergrated with spring!!!! Running at port 8080

Done

