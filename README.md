# react-spring-integration
Integratie the react.js frontend and spring boot backend

1.) Backend - Spring Boot App Setting 

Create Spring Boot App by using Eclipse or Sprint Tool Suit

pom.xml (Default)
￼![alt text](https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/pom.xml.tiff)

Add a TestController for connection test
￼![alt text](￼https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/testController.tiff)


Add a folder named “public” under spring-boot-backend/target/classes/
(This folder is for store react-frontend)
￼￼![alt text](￼https://raw.githubusercontent.com/peterlau0010/react-spring-integration/master/Readme%20Image/add public folder.tiff)


2.) Frontend - React Web Setting

Create React App by running below npm cmd:

Command: npx create-react-app react-frontend
Command: cd react-frontend
Command: npm start
￼


Stop the services, press Ctrl + C

Change react-frontend/package.json setting. Add proxy setting point to your sprint-boot-backend.

￼

Update react-frontend/src/App.js for testing the connection.
￼
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

