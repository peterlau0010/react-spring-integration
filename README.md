# react-spring-integration
Integratie the react.js frontend and spring boot backend

1.) Backend - Spring Boot App Setting 

Create Spring Boot App by using Eclipse or Sprint Tool Suit

pom.xml (Default)
￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/pom.xml.tiff)

Add a TestController for connection test
￼
![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/testController.tiff)


Add a folder named “public” under spring-boot-backend/target/classes/
(This folder is for store react-frontend)
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/add%20public%20folder.tiff)


Run the application, spring boot backend is ready!!!!


2.) Frontend - React Web Setting

Create React App by running below cmd:
```
npx create-react-app react-frontend
cd react-frontend
npm start
```
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/npm%20start.tiff)
Now you will able to see the react js fontend.

Stop the services by press Ctrl + C

Update react-frontend/package.json setting. Add proxy setting point to your sprint-boot-backend.
￼￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/package%20json.tiff)


Update react-frontend/src/App.js for testing the connection.
￼￼![alt text](￼https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/add%20Call%20in%20React.tiff)

Command: npm start 
(Make sure you spring-boot-backend is up and running) otherwise, you will can error.
￼￼
Stop the services. Ctrl +C

Command: npm run build
￼

Check the react-frontend folder structure that contain build folder
￼

3. Integrate two projects

Copy all the files/folders inside react-frontend/build to spring-boot-backend/target/classes/public

￼
Restart the spring-boot-backend App.
￼
Done

