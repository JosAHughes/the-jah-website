# the-jah-website

This project will be a practice / development website to hone my skills and understanding of React, Express, Node, and MongoDB; The MERN Stack.
I will also use this project to hone my skills and understanding of JavaScript, HTML, CSS, and XML.

This project will contain both a client-side web application and a server-side web application.

## This project is to be run on the local machine

### 1: Dependencies -
    - Node.js
    - Express
    - Vite

### 2: Version List -
    - nvm: 1.1.12
    - node: 22.1.0
    - npm: 10.7.0

### 3: Initial Setup Process (for a Windows system) -
    - 1: Install Visual Studio Code (https://code.visualstudio.com/ or use The Microsoft Store)
    - 2: Install git (https://git-scm.com/downloads)
    - 3: Install nvm-windows (https://github.com/coreybutler/nvm-windows/releases)
    - 4: Install node and npm by running, in Command Prompt (since nvm-windows currently won't run in the git bash terminal):
        ```
        $ nvm install node
        ```
    - 5: Run, in Command Prompt:
        ```
        $ nvm use <VERSION_NUMBER>
        ```
        Where VERSION_NUMBER is the version of node you installed in Step 4, NOT the version nvm
    - 6: Launch the Visual Studio Code application
    - 7: Create a folder for your project and name that folder
    - 8: Open your project folder in Visual Studio Code
        - 8.1 (Optional) Changing the Default Visual Studio Code Terminal
            - 1: Create a new terminal by clicking Terminal > New Terminal
            - 2: Click the downward facing arrow next to the + button in the terminal window, then click "Select Default Profile"
            - 3: Choose your prefered terminal
    - 9: Create a new terminal by clicking Terminal > New Terminal
    - 10: Run, in the Visual Studio Code terminal:
        ```
        $ npm create vite@latest react -- --template react
        ```
    - 11: You should get an output that teels you to run three commands. Run them in the order they are presented. They should be:
        ```
        $ cd react
        ```
        ```
        $ npm install
        ```
        ```
        $ npm run dev
        ```