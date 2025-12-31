

### Application setup
This document explains how to prepare the environment and install the application. It covers database setup (creating the `ims` and applying the initial schema), required software (Java 17 and Node 22), copying application files, creating the invoices folder, and starting/stopping the application. Use the quick verification tests below to validate key steps after installation.

## Database Installation
- Install postgress
- Create databse with name `ims`
- Download the initial schema and seed script: <a href="./day_00_script.sql" download="day_00_script.sql">Download day_00_script.sql</a>.
- Run script against `ims`

## Application Installation

### Software
- Create root folder. e.g. C:\OnlineApp
- Extract runtime.zip from \\package folder to \\root folder
- Extract server.zip from \\package folder to \\root folder
- Extract ui-app.zip from \\package folder to \\root\server\html folder
- Copy RetailProcessor-1.0.0.jar to \\root\server\processor folder
- Update \\settings\root.bat with root folder path 
  - set "APP_ROOT=**C:\OnlineApp**"
    
#### Start Application
- Open command prompt and go to application root folder e.g. C:\OnlineApp
- Run command  `start-application.bat`
- Open browser outside server and open url `http://<server-host>:<port>`

#### Stop Application
- Open command prompt and go to application root folder e.g. C:\OnlineApp
- Run command  `stop-application.bat`
