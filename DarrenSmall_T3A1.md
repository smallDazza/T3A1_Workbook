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
- Overview: A MERN stack application is a 