# T3A1 Workbook

## Question 1 Answer:
A standard source control process for a large project will be based on what source control system the project development team are currently using and would most likely be the mostly used VCS system of Git and then the mostly used Git repositories of GitHub or Bitbucket. This VCS software is used by the development team to manage changes in the projects source code over the length of time the project takes to complete.
The development team process for the VCS of the project will be applying a number of standard practices, these are:

    - Repository Setup: organising the structure of the code into clear and consistent repositories.
    - Branching Strategies: to manage code changes a good branch strategy is required. This could be having a 'main' branch for production ready code, a 'dev' branch for ongoing developement and testing, then creating new branches as required for future version releases or bug fixes where these can be merged back into the main branch when finished.
    - Commit Messages & Frequency: when team members are commiting changes they need to write concise and informative messages. This way other members of the team will know and understand what they have done. Members should also be instructed to make regular frequent small commits rather than infrequent larger commits. This makes tracking changes and identification of bugs easier for all team members.
    - Review Of Code: code review practices should be implemented for team members to catch errors, share knowledge and check the code quality adheres to current best practices & standards.
    - Using Pull Requests: team members should use pull requests for all code changes. These pull requests can be used for reviewing code, testing and code quality reviews before merging them back into the 'main' branch.
    -  CI/CD Processes: a Continuous Integration/Continuous Deployment process should be implemented. This involves a pipeline to trigger the automation of the building, testing and deployment of code changes to the dev environment.
    - Resolving Conflicts: all team members should work together to resolve any merging conflicts quickly when they happen. These conflicts happen when different members have modified the same part of a file.
    - .gitignore File: To specifically have any file or directories ignored by the VCS software, member should use a .gitignore file.
    - Security: access control measures should be used by the dev team to protect the main production branch. This security should help prevent things like deletions, direct pushing to production and unauthorised access.
    - Cleanup Process: a branch cleanup process should be regularly done to remove old & unused branches. This will maintain a managable and clean repository.
    - Documentation: The repository should include a documentation file or README file to guide any new or current dev team members of the processes of building, running, testing and cloning any part of the software project.

References:

Atlassian, 2024. What is version control? [Online]
Available at: https://www.atlassian.com/git/tutorials/what-is-version-control

Masal, B. 2023. Best Practices for Effective Source Control (version control) in Software Development. [Online]
Available at: https://www.linkedin.com/pulse/best-practices-effective-source-control-version-software-balaji-masal-agxpf

## Question 2 Answer:
There are a number of important aspects to quality software, these are:
1. Reliability: Software must be available for use all the time and able to perform as expected and still function under heavy usage loads. This also includes the ability to recover quickly and efficiently should faults or failures happen. The best way to achieve reliability is through testing and debugging methods to ensure it functions as intended and if any errors are detected they can be resolved before released to a production environment. 
    - A demonstration example of this would be if a software server goes down, then the software system needs to automatically changeover to another duplicate server to continue the reliability and functionality of the software program.
2. Usability:   This aspect refers to the end users experience when using the software or its User Interface (UI). The UI should be easy to understand and use for all types of end users, from experienced to novice users. This is achieved in the UI design which should be organised in a way that makes it easy to find what the user is looking for, read and understand all text displayed and any buttons easily accessible for selection.
    - A demonstration example of this would be in a ecommerce website, for allowing customers to do refunds/returns, would be making sure the button to allow this is in a prominent position next to each of the customers ordered items. Not in a obscure different area that is not related to the customers ordered products. 
3. Portability: For this to be achieved the software must be available for use on all different types of environments containing different hardware or operating systems. This is most commonly required for use in mobile applications where the software would need to function and render in both Android and IOS environments.
    - A demonstration example of this would be for a application to work on both Android and IOS mobile environments, would be to use cross-platform development frameworks like Flutter or React Native. These tools allow you to write a single codebase that works on both platforms, saving time and resources.
4. Maintainability: This refers to how easily the software can be maintained and updated when developers are wanting to add new features or update existing features. Good software design architecture is required for this aspect with principles being used such as reuse of code and modularity, which will make it easier to modify and update the software code.
    - A demonstration example of this would be the development team using a VCS system such as Git/GitHub. This way the main source code is confidently always updated and documented with the different versions everytime a new version is released. 
5. Efficiency:  The performance efficiency of the software is very important as this is how quickly and accurately it performs the tasks required. To achieve this good effective coding principles and techniques need to be achieved to avoid errors that can slow the system down. Also the efficiency on the system resources such as CPU usage, memory and disk space need to be considered and monitored when the software is being used.
    - A demonstration example of this would be the dev team using coding principles such as KISS (Keep It Super Simple) & DRY (Dont Repeat Yourself) for the simplest coding solutions and removing duplication for a clean codebase. Also using a powerful software development approach like the Test Driven Development (TDD) approach, which involves a short, repeatable development cycles, will greatly improve software efficiency.
6. Security:   One of the most important aspects in the quality of software is its security and its ability to ensure it is safe from unauthorised access, data deletion and data tampering. Ensuring authentication, authorisation and data encryption coding techniques are used to ensure the entegrity of the software data and controlling who has access to this is very important.
    - A demonstration example of this would be if the software has an API endpoint that is exposed to the public. To secure this endpoint and the software system from unauthorised access, the use of a JWT security token should be implemented so only authorised user with the security token can gain access to the endpoint & system.

References:

Geekforgeeks, 2024, Software Quality – Software Engineering [Online]
Available at: https://www.geeksforgeeks.org/software-engineering-software-quality/

Testsigma, 2024, What are the Software Quality Attributes? [Online]
Available at: https://testsigma.com/blog/software-quality-attributes/

Lasting Dynamics, 2022, Software Quality: 8 essential Approaches you need to know [Online]
Available at: https://www.lastingdynamics.com/blog/software-quality-8-approaches/

## Question 3 Answers:
A standard high level structure of a MERN stack application would be as follows:
- Overview: A popular full stack used for web applications is a MERN stack. This is a powerful javascript stack which allows developers to build scalable web applications and contains the four technologies of MongoDB, Express.js, React.js and Node.js.
These four technologies work together to create a three tier architecture pattern called Model View Controller (or MVC). The Model component is the database tier for managing and storing data. The View is the component for displaying the data or front end tier. The Controller is the back end tier and component used for handling user input and updating both the Model & View components as required. All techs use javascript & JSON format which all combine together as in this image and explanation:
    - ![MERN Stack](./images/MERN%20stack.png)
    - Front End Tier;
        - React.js: React is a javascript library that allows developers to build front end user interfaces (UIs) for web applications. It does this by using individual pieces called components, written in javascript, and then combined to render and update as the applications data changes. 
    - Back End Tier;
        - Express.js and Node.js: These both use javascript and work together by running the Express framework inside a Node server. Node.js is used to create a server side environment which will offer back end application functionalities like creating API's, automation & scripting and real time streaming app services etc. Express is a small framework that sits on top of Node.js and enables web application functionality to handle a variety of different HTTP requests. Express also is customisable and permits integration tools and features from other third parties. Both these combined create a seamless back end connectivity environment that is highly scalable and effiicent. 
    - Database Tier;
        - MongoDB: Is a NoSQL database where data is stored in flexable JSON like documents. This document model maps to javascript objects in the applications code. So user JSON documents created in the React.js front end UI can be sent to the server and provided they are valid, will be processed by Express.js and stored directly in the MongoDB database where they can be retrieved later when required.

- MERN Stack Project Structure: Project structure using the MVC architecture pattern is organised in a way that separates the front end code from the back end code. Doing this creates a well organised and maintainable project code structure that improves readability for time saving development but also allows greater future scalability. This is done by creating separate directories for both client side and server side components.
    - Client Side Structure: The client file directory will contain all files and code relating to the front end tier of the application. These could be in a structure like this:
        - Client directory:
            - public folder: This contains files relating to images, fonts and HTML. The index.html file would be located here which is the entry point for React.js.
            - src folder: This file contains the main source code for the front end of the application. Its sub folders & files would be:
                - components: Contains reusable UI components for use across multiple application pages.
                - pages: Each application page can have its own designated folder here with code and logic specific for that page.
                - services: This file will contain all files and code used for services like API functionality and data fetching.
                - utils: Any helper or utility files required can be placed in this folder.
                - App.js file: This file is a container for global initialisation and routing by React.js.
                - index.js file: React.js uses this file for rendering and mounting it into the DOM.
                - .env file: This file contains the environment specific configurations. For EG; database credentials, API Keys.
                - package.json file: This file can be used for adding & running scripts for testing and starting the server.
    - Server Side Structure: The server file directory will contain all files and code relating to the back end tier of the application. These would be in a structure like this:
        - Server directory:
            - config: This holds the back end configuration files, such as environment variables and database connection settings.
            - controllers: This folder will contain the files for each controller route which conatins the logic for handling http requests and data processing.
            - models: Database schemas can be contained in this folder. Each model file contains specific data structure and controls the interactions with the database.
            - routes: The applications API routes are located in this folder. These files are responsible for defining each routes endpoints, mapping them to the correct controller functions and handling the request authentication and validation.
            - server.js file: This is the back end entry point for the Express server and establishing the middleware configs and database connections.  
            
References:

MongDB. 2024. MERN Stack Explained. [Online]
Available at: https://www.mongodb.com/resources/languages/mern-stack

Amankwah, K. 2023. MERN Stack Project Structure: Best Practices [Online]
Available at: https://dev.to/kingsley/mern-stack-project-structure-best-practices-2adk

Alwis, L. 2023. Structuring Your MERN Stack Project: Best Practices and Organization [Online]
Available at: https://masterlwa.medium.com/structuring-your-mern-stack-project-best-practices-and-organization-5776861e2c92

## Question 4 Answers:
In developing a website for a small business the team will need the following knowledge and skills to develop the project:

1. Client Interaction, Research and Planning:
    - 
2. Designing:
    - 
3. Building and Maintaining:
    -
4. Testing:
    - 
5. Communication and Teamwork: