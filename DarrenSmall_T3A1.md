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
There are many different aspects required for developing a website for a small business. Overall the team will need some or all of the following knowledge and skillsets to develop the project:

1. Client Requirements and Research :
    - First steps in any project is a team member(s) will need to have the abilities to sit down and have a meeting with the client and put together a project website brief for meeting all the clients expectations for their website. The planning for this project brief will need to include the following aspects:
        - Identify the goals and objectives of the website. For example what problems is this website going to resolve ?
        - The clients website requirements will need to be defined. These will be a list of the clients requirements, user requirements and outcomes, considering any business industry standards, any market research to be conducted, and if required any third party integrations. 
        - Will need to define the project scope. This project scope is a roadmap of the entire project plan and will include all the functions, contraints and exclusions required.
2. Project Planning:
    - The knowledge and skillsets required in this stage are based on the outcomes in step 1, which is to document a project plan. This plan will include important aspects like:
        - Choosing an appropriate project management methodology that aligns with the project requirements and scope. Will the project be agile or waterfall ? if agile what type of framework will suit the development team, Scrum , Lean or Kanban ?
        - Performing a project risk assessment is also very important. This will evaluate the likelihood and impact of any potential risks and challenges that could affect the projects succesful outcome, while also developing contingency plans if these were to happen.
        - Task management and scheduling of the project will enable the team better progress allocation of resources, task completion dates, estimation of task outcomes and an overall tracking of the entire project for dev team and client management.      
3. Legal Obligations & Project Costings:
    - These next two aspects may or may not be something the actual development team can perform and if not, then outside third party professionals will need to be consulted.  Based on stage twos outcomes the costings will need to be quoted and provded to the client for projects approval and go ahead. Any legal obligations that the clients business has to conform with will also then have to be reflected and added to the projects planning and scope, as this will reduce or negate any future legalities casued by the clients website. 
4. Designing:
    - The dev team will need to have the knowledge and ability to perform the websites UX / UI design. The development team should know the user experience (UX) and user interface (UI) design principles, as this will impact on the users engagement and outcomes. Its important to create a website that is both visually appealing and easy to use.
    - The dev team will also need to have the skillset of building design charts/diagrams for the project. These are important for the projects requirements and building development for the next stage. Examples of these could be use case diagrams, website flowchart for the processes of the website. Commonly used UML diagrams such as Class diagrams and Sequence diagrams will be required for the actual coding of the project. If the website is storing user data then a ER Diagram will also be needed for the building of the database. 
5. Building and Maintaining:
    - This stage is where the developement team members will actually code or build the projects website. The knowledge and skillsets required here by the dev team will be:
        - Proficiency and skill in programming languages. The developers will need to be proficient in programming languages like HTML, CSS, and JavaScript, as a good understanding of these languages is essential for creating and maintaining the website.
        - Knowledge of frameworks and libraries. Besides the programming languages, the developers should be familiar with frameworks and libraries like React, Angular, or Svelte. These tools make it easier to develop and can help the development team save time and effort on building the website.
6. Testing:
    - The dev team here will require testing and debugging skills. Before going live and releasing to the client, developers will be required to test and debug their code to ensure the website functions correctly. This requires attention to detail and the ability to identify and fix errors in the code.
7. Communication and Teamwork:
    - Overall the knowledge here for the development team as a whole, and also as individuals, will need to work collaboratively as a team. Team members should have strong communication and teamwork skills. They should be able to work in a team environment but also trusted and the abilities to work alone on tasks as required.

References:

Katz, I. 2024. Website Design For Small Business: The Ultimate Guide. [Online]
Available at: https://www.web4business.com.au/portfolio-item/website-design-for-small-business-guide/

Nova, S. 2023. 7 Must-Have Skills for Building a Winning Website: A Developer's Guide [Online]
Available at: https://www.linkedin.com/pulse/7-must-have-skills-building-winning-website-developers-guide

## Question 5 Answers:
The knowledge and skills required for a work project I was invloved in and the challenges I had to overcome are mentioned below:
- The Work Project: A couple of years ago in the current company I am employed with, I was asked to join the product management team to work on a new project of building a new cloud software application based on the companies current dot net windows software application.
- Knowledge & Skills Required: The knowledge and skills required for my part in the project was the following:
    1. Software workflow knowledge of the current application and how this will need to be similarly transitioned across to the new cloud application.
    2. Documentation skills for the workflow of the new cloud application and how this can be improved, based on current software application customer feedback and complaints.
    3. Based on the knowledge of current software application UI / UX design, contribute to the design and documentation of the new cloud applications UI / UX features.
    4. Knowledge of the current third party software integration partners and how the data from these interact with the data of our current software application.
    5. Document, advise and improve on how the data from these software integration partners will be handled in the new cloud application.
    6. Task management program knowledge and skill that the development team were using, which was the Atlassian program of Jira. 
    7. Communication skills in both writing and speaking with meetings of the different groups invloved in the project being the Dev team, company management, integration partners and customers involved in beta testing.
    8. Team work knowledge and skill to work together with all the different aspects and personalities that come with multiple different team members to see the project outcomes achieved in the project areas I was invloved in. 
- Challenges To Overcome: With my background being from leading the current software training team and managing client software requests there were a number of new challenges I had to work through in my new role on the project management team. These were:
    1. Documentation: Specifically researching and learning how to document the workflow for the new cloud application, by the way of diagrams & charts, so the dev team would be able to interpret these correctly. These mostly were UML software behavioral diagrams such as use case, activity diagrams and flowchart diagram.
    2. Design: This was the most challenging aspect for me, as I had never been involved in any sort of designing features or UI / UX design and functionality before. Therefore i was more like a junior in helping in this area and took my instructions and learning from more experienced team members. The areas mostly helped out with here were the initial cloud applications site mapping and appliction page wire frame layouts to be very similar or improved on from the current software.
    3. Integration Data: A couple of our integration partners advised our dev team that they had now created and developed new API endpoints for our software to use and move away from the current SQL database connections our current software was using. So the project manangement and dev teams decided to incorporate these new endpoints into the new cloud application. Having at the time no software developemnt or coding experience, the only understanding I had (from just years of experience) was the basic SQL data fields & formats used for these integration partners. So this was another on the job challenge and learning from the dev team members of how to use the Postman and swagger programs to check the API endpoint data we were given access to, was correct for use in the cloud application.

## Question 6 Answers:
In the above project mentioned to evaluate the effectiveness of my knowledge and skills mentioned with examples and then to provide an improvement would be as follows by the numbers mentioned above:
- Numbers 1 & 2:  My knowledge of the workflow of the current software program after years of training customers and then managing the training team, was being one of the most experienced members in knowledge of the current app in the project management team. For example: I was asked to explain and document the workflow process for a user to import a patient and all their scripted medications from all of our different integration partner programs into our current software program and then recommend the same processes or improvements to be done in the cloud application.
    - An improvement here would be in my presentation, because of my in depth knowledge of all the integration partners and the processes, not skip over the basic things and presume most of the team members already know these processes as I do, but to explain and communicate the complete process. As I found myseld on a number of occasions having to revisist basic item functions that I skipped over as this at first didnt make sense to some attendies that were at a basic or mid level of software workflow knowledge.

- Number 3: As mentioned in the Q5 challenges area, designing something is not my strongest attribute, so I was not very effective in the actual UI design and layout of the new cloud app. From my experience in dealing and training customers on the current app, I was more effective in providing the new cloud app layout for UX design and functions. For example:  In the image below, the both apps 'Patient Pack Management Areas', the UI design looks better in the new cloud app (not that I had much feedback here) , whereas the UX design functions in the new cloud app still provide the same entire interaction  outcomes required in both apps (my involvement). 
    - An improvement here would be knowing more about UI design particularly in web development. Things like the program screen layout of the displayed text data, buttons, icons, images and then how to use the correct colour palettes to combine all these items together in the web browser environment would be an excellent skill and knowledge to know for any future similar projects. This is one reason why I decided to do this coder academy course.

![App Pack Management](./images/Q6-a.png)

- Numbers 4 & 5: The effectiveness of my knowledge here for our integration partners and how we currently access their data was important and very effective for the dev team to apply to the new cloud application. However my skills in knowing how to access the new API endpoints provided by the integration partners for the cloud app was lacking and required training. The dev team did help and provide on the job training for me to improve my skills and know how to do this. For example: based on the API endpoint documentation from the integration partners, using the Postman program, we had to confirm the data we had access to was correct for what our cloud application required.
    - An improvement here would be more training and skills in knowing about API endpoint and http request functionalities. As most web applications use this type of functionality for fetching data from third party integrations, knowing how to use multiple http request programs would be highly admired for working on any future similar projects. This is another reason why I decided to do this coder academy course. 

- Numbers 6,7,8: The effectiveness of my knowledge & skills for all three points here was satisfactory based on my previous experience. Being prevoiusly employed in a software support role where a couple of similar task managemnt programs were used, it was relatively easy to transition over and use the Jira program that the project management team were using. Also then being invloved in a couple of different teams, from support and then training over many years, was very familiar for me to join and work within the new project management team. So therfore i did not have any issues in my role or working with other team members.
    - An improvement here would be always to increase and move forward with personal communication skills and even further to develop and train for leadership skills. This is a skill we can always improve on to meet the challenges of working within a team where a wide range of different people and their personalities are involved and team leadership would always be a desireable for any future similar projects.

## Question 7 Answers:
Control flow in the Javascript language is the order in which the interpreter executes statements. Code is executed from top to bottom unless a / set of statement(s) changes the control flow. This control flow is divided into two main control flow construct categories of conditional statements and iteration statements: 
- **Conditional Statements.**

These statements evaluate a certian condition or set of conditions and then execute the code it contains if the evaluated condition(s) equal True, otherwise the code is skipped. The types of conditional statements are:

```
- If Statement: An if statement evaluates the condition in its parenthesis and if this condition is true, will then execute the following code contained in the curly braces. The code is ignored if the condition evaluates to false. An example of this statement is: 


    var isRaining = true;
    if (isRaining) {
        alert("Don't forget an umbrella!");
    }
```
```
- Else Statement: An else statement cannot stand alone, but if required, will follow a preceding if statement. The else statement will only execute the following code when the preceding if statement condition evaluates to false. An example of this statement is:

    var isRaining = true;
    if (isRaining) {
        alert("Don't forget an umbrella!");
    } else {
        alert("No need for an umbrella.");
    }
```
```
- Multiple Else, If Statements: To chain multiple if statements together, the next if statement syntax will be expressed by using a combination of else if and then the condition in parenthesis to be evaluated, with the code to be executed in the same curly braces should the condition evaluate to true. The code is ignored if the condition evaluates to false. An example of this statement is: 

    var isRaining = true;
    if (isRaining) {
        alert("Don't forget an umbrella!");
    } else if (isSunny) {
        alert("Wear a wide hat !")
    } else {
        alert("No need for an umbrella or a hat today, just be comfortable!");
    }
```
```
- Switch Case Statements: similar to else if statements a switch statement can be used to evaluate a condition once and then if any of the following case statements match the condition, that particular case code will be executed. To stop evaluating the swtich body when a case is a match, the break keyword is added after the case code. Should none of the cases be a match then a default statement can be added and its code executed should the switch case statement be undefined. An example of this statement is:

    switch ( 20 ) {
        case 5:
            console.log( "The value was five." );
        break;
        case 10:
            console.log( "The value was ten." );
        break;
        default:
            console.log( "The value was something unexpected." );
    }
```

- **Iteration statements.**

These statements are usually referred to as loop statements and execute code repetitively until either one or more conditions are met, or no longer met, depending on the type of loop statement used. Loop statements interupt the top to bottom code execution, until the loop ends, then the control flow again executes the next statements after the loop. Here are some of the most used types of iteration statements:

```
- For Loop: this is the most common type of loop for repeating code a known number of times, while a condition is true. Its syntax is to use the word for, then inside a set of parentheses, has these 3 sets of expressions:
    1. initialisation: this defines & initialises a variable.
    2. condition: this must evaluate to true for the code to be executed (loop to continue).
    3. modification: a expression to be executed at the end of each loop.
    After this is the code to be executed inside a set of curly braces for each iteration.An example in code of a for loop is:

    const food = ['Pizza', 'Pasta', 'Burgers']

    for (let i = 0; i < food.length; i++) {
        console.log(food[ i ])
    }
```
```
- While Loop: this loop will also repeat while a condition is true but not sure how many times to do this. Its syntax is to use the word while, then inside a set of parentheses the condition to be evaluated after each loop, then the code to be executed inside a set of curly braces for each iteration. So long as the condition is true the while loop will keep iterating. An example in code of a while loop is:

    let countNumber = 0;

    while( countNumber < 4 ) {
        countNumber++;
        console.log( `Number is ${ countNumber }.` );
    }
```
```
- Do While Loop: This is simply a different variety of while loop with the difference being the condition to be evaluated is at the end of the loop. This means one loop iteration is always completed before the condition is evaluated. The syntax for this is the addition of the do word, with the same while loop syntax but in different positions, an example in code like this:

    let countNumber = 0;

    do {
      console.log( `Number is ${ countNumber }.` );
      countNumber++;
    }
    while( countNumber < 4 );
        
```
References:

Codeguage. 2024. JavaScript Control Flow [Online]
Available at: https://www.codeguage.com/courses/js/control-flow

Cleary, R. 2020. Control Flow in Javascript [Online]
Available at: https://medium.com/@rianna.cleary/control-flow-in-javascript-9c63d0c98bb9

Web.dev, 2024. javascript Control flow [Online]
Available at: https://web.dev/learn/javascript/control-flow

## Question 8 Answers:
Type coercion in the Javascript language is its ability to convert values from one type to another, such as number to string, string to number, boolean to number etc. Because javascript is a loosley typed language, it is always looking to help out or find common ground when the code has different types of data brought together.This process to transform types can happen in two different ways by implicit coercion or explicit coercion:

**Implict Coercion.**

- This is where javascript does the type coercion automatically behind the scenes. This happens when operators are applied to values, such as string concatenation of joining string values and number values, and also happens by the surrounding code context, for example in a if statement where the value in parentheses is coerced to a boolean value.
- **Comparison Operators:** There is a comparison operator that when used will not allow implicit type coercion to happen. The strict equality operator of ' === ' will not allow this to happen. But on the other hand if using the loose equality operator of ' == ', this will be different and allow type coercion and comparison if required. Therefore in most cases it is recommended to use the strict equality operator and reduce surprising outcomes in code output.

A code example of implicit coercion:
```
    let number = 55;
    let result = "Your number is: " + number;
    console.log(result);
    // the result is all as a string:  "Your number is: 55"
```

**Explicit Coercion.**
- This is where the developer explicitly in code uses javascripts built in functions to intentionally convert the types. This is most useful when the developer does not know the type of a value the code is expecting, like for example data coming from an API. Some of these javascript functions to explicitly convert are:
    - To a string type: String()
    - To a number type: Number()
    - To a boolean type: Boolean()

For example using a number value expected from an API, could be as a string type. So to then use this number with other number types in the code, the Number() will need to be used to explicitly coerce the string to a number.EG:
```
const apiNumData = {
    value: "250"
}

const myNum = 100;
const value = Number(apiNumData.value);
result = myNum + value;
console.log(result)
// the result is: 350
// because the "250" string type is explicitly coerced to a number type using the Number().
```
References:

Rahman, S. 2024. Type Coercion in JavaScript: A Comprehensive Guide [Online]
Available at: https://www.linkedin.com/pulse/type-coercion-javascript-comprehensive-guide-shourav-rahman-faelc

freeCodeCamp. 2022. Coercion and Type Conversion in JavaScript [Online]
Available at: https://www.freecodecamp.org/news/coercion-and-type-conversion-in-javascript/

## Question 9 Answers:
Javascript data types are the different types of data that the code will be working with and storing in variables. Its important to note that in javascript the types are dynamic, meaning the same variable can be used to hold different data types. There are 8 data types in javascript and these are divided into two categories of primitive and non primitive data types.

**Primitive Data Types:** These are predefined by the javascript language and can hold a single value, also be known as in built data types.

 - Number: this number data type uses a unified approach for all numeric values. It uses the numeric type double-precision 64-bit binary format IEEE 754, which means there is only one numeric type used, no difference between a integer and float types. An example of this is:
 ``` 
    // With decimals:
    let x = 34.50;

    // Without decimals:
    let y = 34;
```
 - String: this data type is a sequence of characters mostly used to represent text. The syntax for a string is to use either single or double quotes and like other programming languages the string data type is immutable. An example of this is:
 ```
    // Using double quotes:
    let carName1 = "Ford Ranger is a great 4WD";

    // Using single quotes:
    let carName2 = 'Ford Ranger is a great 4WD';
```
 - Boolean: this data type represents true or false values. The value of '0', 'NaN', an empty string, 'undefined', and 'null' are all treated as boolean false values. Number values other than 0, non empty strings, a variable or object that has a value are all treated as boolean true values. An example of this is:
 ```
    let x = 5;
    let y = 5;
    let z = 6;
    (x == y)    // Returns true
    (x == z)    // Returns false
```
 - BigInt: this data type is used to store big number values that are to big for the number data type. The number data type is only accurate up to a total of 15 digits, numbers bigger than this will require the BigInt data type. The syntax for this is either append a 'n' to the end of a number or use the BigInt(). An example of this is:
 ```
    let x = 1234567890123456789012345n;
    let y = BigInt(1234567890123456789012345)
```
 - null: the null data type represents the absense of any value or is used as a placeholder for an object value that is not present as yet. An example of this is:
 ```
    const test = null;
    if (test) {
    console.log("test is not null");
    } else {
    console.log("test is null");
    }
    // the result is: "test is null"
```
 - Undefined: this data type in javascript is by default assigned when a variable is declared and not initialised or not assigned a value. Functions can also return a undefined value, if a variable was assigned to that function and the function does not return any value, the variable will be assigned a undefined value. Examples of these:
 ```
    let variable = undefined;
    // or
    let x; 
    // both will contain a undefined value.
```
```
    function hello(name) {
        console.log(`hello ${name}`);
    }
    x = hello('Mike');
    console.log(x);
    // the x variable will be assigned a undefined value because the function does not return anything
```
 - Symbol: this data type is unique and immutable and can be used to add a unique property key value to an object. Because it is unique this will not collide with any other keys that could be added to the object. The syntax to create a symbol is Symbol() which can also pass a optional string value. An example is:
 ```
    let value1 = Symbol("value");
    let value2 = Symbol("value");
    console.log(value1 === value2); 
    // this results in false
```

 **Non Primitive Data Types:** These are derived from primitive data types and can hold multiple values.

 - Object: this data type is a data structure and used to store data collections. The data is stored as key value pairs where each key is a unique identifier for its assigned value. These objects can have there properties added, changed or deleted at runtime which makes them dynamic. The syntax to create an object is by using curly braces to define the object and initialising the properties as key value pairs, separated by a comma.EG:
 ```
    let obj = {
    name: "Mike",
    age: 28,
    job: "Developer"
    };
    console.log(obj);
    // the result is { name: "Mike", age: 28, job: "Developer" }
```
- The same object can be created by also using the Object():
```
    let obj = new Object();
    obj.name= "Mike",
    obj.age= 28,
    obj.job= "Developer"

    console.log(obj); 
```
- Object; 'Array': another special kind of object is an array. This is used to store an ordered collection of values and can be of any data type. The syntax for an array is using square brackets [], with values separated by a comma.EG:
```
    let x = [1, 2, 3, 4, 5, "one", "two", "three"];
    console.log(x);
    // result is [1, 2, 3, 4, 5, "one", "two", "three"]
```
References:

Programiz. 2024. JavaScript Data Types [Online]
Available at: https://www.programiz.com/javascript/data-types

GeeksforGeeks. 2024. JavaScript Data Types [Online]
Available at: https://www.geeksforgeeks.org/javascript-data-types/

Shiksha. 2023. Introduction to JavaScript Data Types With Examples [Online]
Avialable at: https://www.shiksha.com/online-courses/articles/javascript-data-types-with-examples/#sym

## Question 10 Answers:
In javascript arrays are dynamic meaning the element values can be changed, removed or new values added once they have been created. Arrays can be manipulated by using many different kinds of methods. These methods can manipulate the existing array they have been called on or some of these methods will return a new array and then populate it with the same or changed elements, keeping the original array but with the new and original array having the same reference. The syntax for using these methods is by after the array name using a dot and the method name with any values in the method parentheses.

**Some of these methods that manipulate the existing/original array are:**
- .push(): this method is used for appending (adding) a new element value to the end of an array. Example:
```
    let evens = [2,4,6,8];
    evens.push(10);
    
    console.log(evens);
    // result to array is number 10 added to the end: [2,4,6,8,10]
```
- .pop(): this method is used for removing the element that is located at the end of the array. Example:
```
    let odds = [1,3,5,7];
    numbers.pop();

    console.log(odds);
    // the result is number 7 removed: [1,3,5]
```
- .splice(): this method can be used for removing elements at a certain location(s) and also adding new elements at the location(s) of the removed elements. Example:
```
    let animals = ['whale', 'tiger', 'shark', 'horse', 'bird'];
    animals.splice(1,3);

    console.log(animals);
    // result is the elements located at position 1 to 3 ['tiger', 'shark', 'horse'] are removed. The original array is:  ['whale', 'bird']

    // to remove & add to the same array:

    animals.splice(1,3,'cats', 'dogs');
    
    console.log(animals);
    // result is the elements located at position 1 to 3 ['tiger', 'shark', 'horse'] are removed & replace with the element values 'cats', 'dogs'. The original array is now:  ['whale', 'cats', 'dogs', 'bird']

```
**Some of these methods that will return a new manipulated array (keeping the original) are:**
- .concat(): this method is used for adding element(s) to the end of an array, including merging two or more arrays together. A couple of example are:
```
    let cars = ['ford', 'holden', 'toyota', 'suzuki']
    let newCars = cars.concat('mazda');
    console.log(newCars);
    // result is a new array with: ['ford', 'holden', 'toyota', 'suzuki', 'mazda']
    // merging 2 or more arrays:
    const array1 = [1, 2, 3];
    const array2 = [4, 5, 6];
    const array3 = [7, 8, 9];

    const mergedArray = array1.concat(array2, array3);
    // mergedArray is [1, 2, 3, 4, 5, 6, 7, 8, 9]
```
- .map(): this method can be used to transform and return the same number of elements as the original array. Example:
```
    const drinks = ['Coca-Cola', 'Pepsi', 'Sprite', 'Creaming soda']
    drinks.map(newDrinks => {
        let i = 0
        if (newDrinks[i] === 'C') {
            newDrinks = 'Fanta';
        }
    console.log(newDrinks)
    })
    // the new array returned is:  ['Fanta', 'Pepsi', 'Sprite', 'Fanta']
    console.log(drinks)
    // But the original array is still available: ['Coca-Cola', 'Pepsi', 'Sprite', 'Creaming soda']
```
- .join(): this method does not return a new array but will join all the elements in the original array and return them as a new string. This method can also take a optional seperator parameter but by default will use a comma as the seperator. Example:
```
    const array = ['apple', 'banana', 'orange'];
    const fruitString = array.join();
    // result is a string:  'apple,banana,orange'

    // with a seperator as a parameter:
    const array = [1, 2, 3];
    const numberString = array.join('-');
    // result is a string: '1-2-3'
```
References:

Ayodeji, B. 2019. How to Manipulate Arrays in JavaScript [Online]
Available at: https://www.freecodecamp.org/news/manipulating-arrays-in-javascript/

Yerimah, D. 2023. Array Manipulation: Understanding JavaScript Array Methods [Online]
Available at: https://hackernoon.com/array-manipulation-understanding-javascript-array-methods

Mdn web docs. 2024. Javascript Array [Online]
Available at: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

## Question 11 Answers:
As mentioned in question 9 an object is a collection of key value pair properties. There are many ways to manipulate a object:
1. You can use the dot or bracket notation (the same as when accessing the value of a property) to either set new or update existing properties.
2. To delete object properties the 'delete' operator can be used.
3. Then javscript also provides many built in methods which can perform actions on a objects properties. The syntax to access these object methods is: objectName.methodName(params).

    1. Examples using the dot or bracket notation to set new properties or update existing properties:
    ```
        let person = {
            name: "Peter",
            age: 28,
            gender: "Male"
        };

        // Setting a new property with dot notation:
        person.country = "Australia";
        console.log(person.country); 
        // result is: Australia
        // Setting a new property with bracket notation:
        person["email"] = "peterparker@email.com";
        console.log(person.email); 
        // result is: peterparker@email.com

        // Updating existing property with dot notation:
        person.age = 30;
        console.log(person.age); 
        // result is: 30
        // Updating existing property with bracket notation:
        person["name"] = "Peter Parker";
        console.log(person.name); 
        // result is: Peter Parker
    ```
    2. Examples to delete a objects properties using the delete operator:
    ```
        let person = {
            name: "Peter",
            age: 28,
            gender: "Male",
        };

        // Deleting a property :
        delete person.age;
        console.log(person.age); 
        // result because the property deleted: undefined
    ```
    3. Calling a objects method can be done using the dot notation. Examples:
    - a method or function inside a object:
    ```
    let person = {
        name: "Peter",
        age: 28,
        gender: "Male",
        displayName: function() {
            alert(this.name);
        }
    };

    person.displayName(); 
    // Outputs: Peter
    ```
    - In javascript there are many object methods to use to manipulate objects, some of them are:
        Object.keys() ,
        Object.values() ,
        Object.entries() ,
        Object.fromEntries() ,
        Object.assign() ,
        Object.seal() ,
        Object.freeze() ,
        Object.preventExtensions() ,
        Object.isSealed() ,
        Object.isFrozen() ,
        Object.isExtensible() ,
        Object.is() ,
    - Example1: using the Object.assign() , this copies all properties across from one or more objects to be combined in a new object:
    ```
    const person1 = {
        name: "Mike",
        age: 25,
        city: "Sydney",
    };

    const person2 = {
        country: "Australia",
    };

    const person3 = Object.assign(person1, person2);

    console.log(person3); 
    //result is a new combined object: { name: 'Mike', age: 25, city: 'Sydney', country: 'Australia' }
    ```
    - Example2: using the Object.freeze() , this method freezes an object which prevents neww property additions, prevents existing properties from being deleted or edited. Essentially this makes the object immutable:
    ```
    const person1 = {
        name: "Mike",
        age: 25,
        city: "Sydney",
    };

    Object.freeze(person1);

    person1.country = "Australia";
    person1.name = "Peter";
    delete.person1.city;

    console.log(person1);
    //result is the same immutable object: { name: 'Mike', age: 25, city: 'Sydney' }
    ```
References:

Tutorialrepublic. 2024. JavaScript Objects [Online]
Available at: https://www.tutorialrepublic.com/javascript-tutorial/javascript-objects.php

Ashiq, M. 2023. Object Manipulation [Online]
Available at: https://dev.to/mrizwanashiq/object-manipulation-1dh6

Singh, G. 2021. Objects manipulation in Javascript (tutorial) [Online]
Available at: https://medium.com/@gurpreet212004/objects-manipulation-in-javascript-tutorial-8dfe5f95c2f5

## Question 12 Answers:
The JSON format is a text format representing data structured in a key value pair format and based on the javascript language hence why its is called Javascript Object Notation. JSON can be manipulated by the javascript language as its syntax is similar to javascript objects with some differences where the JS objects keys are not strings in quotes, where JSON keys are. Again javascript has some JSON methods that allow the manipulation of the JSON format in & out of javascript objects, then the object data can be manipulated as required using the javascript langauge. Some example are:

1. To manipulate JSON format into a JS object we use the JSON.parse(). This method will parse all JSON data into a javascript object, where it can be accessed and modified as required by the javascript language. EG:
    ```
    const jsonString = '{"name": "John Doe", "age": 25, "isStudent": true}';
    const jsObject = JSON.parse(jsonString);
    console.log(jsObject);
    // result is a JS object: 
    {
        name: "John Doe",
        age: 25,
        isStudent: true
    }
    ```
2. To convert a javascript object back into a JSON format string we use the JSON.stringify(). This is very useful for transpoorting the data to a server or saving the data locally. EG:
    ```
    const jsObject = {
        name: "Mike Doe",
        age: 30,
        isStudent: false
    };
    const jsonString = JSON.stringify(jsObject);
    console.log(jsonString);
    // the result is a JSON format string: 
    '{"name":"Mike Doe","age":30,"isStudent":false}'
    ```
References:

GeeksforGeeks. 2024. How to Create and Manipulatinag JSON Data in javaScript? [Online]
Available at: https://www.geeksforgeeks.org/how-to-create-and-manipulatinag-json-data-in-javascript/

CarlosRojasDev. 2024. JavaScript and JSON: Parsing, Stringifying, and Manipulating Data [Online]
Available at: https://blog.carlosrojas.dev/javascript-and-json-parsing-stringifying-and-manipulating-data-c3c2b406cd1b

Metana. 2024. JavaScript and JSON [Online]
Available at: https://metana.io/blog/javascript-and-json-examples-in-action/















