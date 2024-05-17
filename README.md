# the-jah-website

This project will be a practice / development website to hone my skills and understanding of React, Express, Node, and MongoDB; The MERN Stack.
I will also use this project to hone my skills and understanding of JavaScript, HTML, CSS, and XML.

This project will contain both a client-side web application and a server-side web application.

## This is a local machine project

### 1: Dependencies -
- Node.js
- Express
- Vite
- MongoDB

### 2: Program List (See Initial Setup process Below for Installation Instructions)
- Visual Studio Code
- git
- MongoDB Community Server
- MongoDB Compass
- MongoDB Shell
- MongoDB Command Line Database Tools
- Postman

### 3: Version List -
- nvm: 1.1.12
- node: 22.1.0
- npm: 10.7.0
- mongodb: 7.0.9
- mongosh: 2.2.5
- mongodb cli tools: 100.9.4

### 4: Initial Setup Process (for a Windows system) -
1. Install Visual Studio Code 
    - https://code.visualstudio.com/ or use The Microsoft Store.
2. Install git 
    - https://git-scm.com/downloads
3. Install MongoDB Community Server and MongoDB Compass
    - https://www.mongodb.com/try/download/community
    - Both MongoDB Community Server and MongoDB Compass are installed from the same installer.
    - Keep clicking Next in the installer. We're installing the Complete version with no modifications.
4. Install MongoDB Shell
    - https://www.mongodb.com/try/download/shell
    - Use the msi installer, not the zip
5. Install MongoDB Command Line Database Tools
    - https://www.mongodb.com/try/download/database-tools
    - Use the msi installer, not the zip
    - Follow the installation instructions here to add the tools to the PATH: https://www.mongodb.com/docs/database-tools/installation/installation-windows/
    - If you're like me, the PATH is:
        ```
        C:\Program Files\MongoDB\Tools\100\bin\
        ```
5. Install Postman
    - https://www.postman.com/downloads/
6. Install nvm-windows 
    - https://github.com/coreybutler/nvm-windows/releases
7. Install node and npm 
    - In Command Prompt run this command:
        ```
        nvm install node
        ```
8. Start using node
    - In step 4 the terminal should say which version of node was installed. Use that number to replace VERSION_NUMBER in the command below.
    - In Command Prompt run this command with the correct version number:
        ```
        nvm use VERSION_NUMBER
        ```
9. Launch Visual Studio Code
10. Create a folder for your project
11. Open your project folder in Visual Studio Code
    - 8.1 (Optional) Changing the Default Visual Studio Code terminal
        - 1: Create a new terminal by clicking:
            - Terminal > New Terminal
        - 2: Click the downward facing arrow next to the + button in the terminal window, then click:
            - Select Default Profile
        - 3: Choose your prefered terminal (I chose git bash)
12. Create a new terminal by clicking:
    - Terminal > New Terminal
13. Run this command in the Visual Studio Code terminal:
    ```
    npm create vite@latest react -- --template react
    ```
14. You should get an output that teels you to run three commands. Run them in the order they are presented. They should be:
    ```
    cd react
    ```
    ```
    npm install
    ```
    ```
    npm run dev
    ```
15. Open MongoDB Compass and Connect to localhost:27017
16. Make yourself a Database in MongoDB using MongoDB Compass or the MongoDB Command Line Database Tools
    MongoDB Compass:
    - You will a list on the left hand side that says:
    My Queries
    Performance
    Databases
    - To the right of Databases, there is a circular refresh symbol and a + symbol. Click this + symbol to create a new database. Name it what you want.
    - When you hover your cursor over one of the Databases (by default: admin, config, and local respectively), you will see a + symbol and a trash symbol. Click the + symbol to add a new Collection to the Database your cursor is hovering over.

    MongoDB Command Line Database Tools:
    - IMPORTANT: Have a json file with data ready to import into the Database before proceeding.
    - Use the following command in a terminal, replacing DATABASE_NAME, COLLECTION_NAME, PATH_TO_JSON_FILE, and JSON_FILE_NAME according to your project's parameters:
        ```
        mongoimport --uri mongodb://localhost:27017/DATABASE_NAME --collection COLLECTION_NAME --drop --file c:/PATH_TO_JSON_FILE/JSON_FILE_NAME.json --jsonArray
        ```
17. Open Postman
    - Click the + symbol in the top bar underneath where it says "Search Postman".
    - We'll be using Postman to test GET, POST, PUT, PATCH, DELETE, HEAD, and OPTIONS requests sent to our server.
    - For now, use this URL (http://localhost:3000/api/) in the section that says "Enter URL or paste text". We'll be adding our paths / routes to the end of "/api/" later.