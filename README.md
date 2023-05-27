# MyVault_Application Documentation
a software development project that aims to create a web-based application that allows individuals to capture their  memories, access previously created personal stories whenever they want, modify details or contents of an existing personal memory in the system , and remove permanently their own unique private stories  in a digital environment

### Project Requirements :
- The MemoryVault project is a software development project that aims to create a web-based application that allows individuals to capture their  memories, access previously created personal stories whenever they want, modify details or contents of an existing personal memory in the system , and remove permanently their own unique private stories  in a digital environment, 
- The purpose of the project is to provide users with a tool that can help them increase productivity and efficiency by providing a convenient and secure way to document and preserve personal experiences.
- The expected outcomes of the MemoryVault project are a fully functional web application that users can access from any device with internet access. The application have a user-friendly interface that allows users to create, edit, and organize their notes and tasks in a logical and efficient way. Additionally, the application include features such as categorization, and search functionality to make it easier for users to find and manage their notes and tasks.  These are some specific constraints and limitations of the MemoryVault project:  Security: The application is secured and protect users' data from unauthorized access or breaches. It also implement appropriate security measures, such as password encryption and authentication, to ensure the safety of users' data.
- Pagination: it can deal with large amounts of data from user, it is also able to handle error and catch exceptions that may arise while using application therefore it display the appropriate error messages to the user 
- Performance: My application is fast and responsive, even when dealing with large amounts of data. It optimized the application's performance to ensure that it can handle a high volume of users and data. 
Other constraints is briefly described in project plan 

### Project Plan :
- Project Name:  MemoryVault 
- Project Scope: 
1. Develop a web application called MemoryVault 
2. Allows individuals to capture their memories, access easily and quickly previously created personal stories, modify contents of an existing personal memory in the system, 
and remove permanently their own unique private stories in a digital environment.
3. Implement authentication and authorization.
4. Increase application performance by validating user input, pagination, caching and handling errors.

- Project Timeline: 
#### Phase 1: 
Planning and Requirements Gathering (2 days)  Conduct market research to identify similar apps and potential competition Define project requirements and prioritize features Develop project plan, timeline, and budget
#### Phase 2: 
Design (2 days)  Develop wireframes and prototypes of the app's user interface and experience Conduct user testing and incorporate feedback Design the app's visual branding, including logo and color scheme 
#### Phase 3: Development (3 days)
•	Develop the app's front-end using html, css and java script 
•	Develop the app's back-end using spring framework and PostgresDB
•	Conduct testing and debugging
#### Phase 4: Deployment and Launch (1 day)
•	Deploy the app using Heruko Application 
•	Develop marketing plan and promotional materials Launch the app 


- Project Resources:  
Project Manager UX/UI Designer Developer (frontEnd, BackEnd & Database)                                                                    Quality Assurance Tester Marketing Specialist 
- Project Constraints:
•	Budget: $500,000
•	App must be developed for iOS and Android Platforms.
•	App must comply with all applicable privacy laws and regulations
•	App must be user-friendly and accessible to everyone.

## Source Code
### Source code are provided here on GitHub repository
https://github.com/Sam-Striker/SpringBootMyVault_Application

## Databaese schema

![myDB](https://github.com/Sam-Striker/SpringBootMyVault_Application/assets/85891662/1e219125-fe6f-4f66-847c-08edadfa44aa)

Here is my entities and their relationships
myvault there is one-to-one  relationship where many vault can be accessed by user  and both admin and user can access vaults 
users there is many-to-many  relationship where different users have access to different vaults and depends on roles admin can delete while user can’t
roles  there is many-to-many  relationship mapped to users entity

## User Documentation
Welcome to MemoryVault! This is a powerful web-based application that helps you manage your notes and organize your thoughts in a visual and intuitive way. In this guide, you will learn how to use the application, navigate its features, and make the most out of it.  Getting Started To start using MemoryVault, simply open your web browser and go to the URL of the application [localhost: 8083]. You will be presented with the main screen, which consists of a blank canvas and a toolbar at the top.  You will be redirected to home page where you can get to know more about this application then click on Login, if you have no account you can click on register .

Creating and Editing Notes Stories are the core element of MemoryVault, and you can create as many of them as you need. Each note consists of a title, a content area, and a set of properties that you can customize to your liking.  To create a new story, simply click on the "Create New” button in the toolbar. This will open a new window where you can enter the title and the content of your note. You can customize the appearance of your text, including fonts, colors, and styles.  You can also add images by using the "choose file" menu.          This will allow you to upload files from your computer or external sources on the web. 
- To view an existing story, simply locate it in my vault section then on right side click on the "view" button in the toolbar. This will open the note in view mode, where you can view it as one.
- To update an existing story, simply locate it in my vault section then on right side click on the "edit" button in the toolbar. This will open the note in edit mode, where you can make changes to its content and properties then save. 
- To delete an existing story, you have to be logged in as admin simply locate story and then click on the "delete" button in the right corner. This will open the tab that tells you that the story is deleted as successfully!
 Organizing your stories.  MemoryVault offers several features to help you organize your story and keep them easily accessible. You can use the following tools to manage your story:  Search: you can search any created story by specify it in search bar.

- Pagination MemoryVault allows you to view many vaults in readable and easily manner where it is sort to 10 when you have above 10 stories you can go to other page.
- Conclusion MemoryVault is a versatile and powerful tool that can help you manage your story and organize your thoughts in a visual and intuitive way. We hope this guide has been helpful in getting you started with the application, and we wish you all the best in your story -capturing endeavors!

## Technical Documentation
Technical Documentation for MemoryVault Project:  Architecture Overview: The MemoryVault application follows a client-server architecture where the client communicates with the server using thymeleaf. 
* The front-end is built using HTML, CSS, and JavaScript, while the back-end is built using java, spring framework and PostgresDB. 
* The user interface is designed to be simple and intuitive, allowing users to create, view, edit and delete story easily. 
* Implementation Details: The front-end of the MemoryVault application is built using HTML, CSS, and JavaScript. Which provides responsive and mobile-first UI components. 
* The front-end communicates with the server using thymeleaf provided by the back-end.  The back-end is built using java, spring framework, which provides a robust and scalable server-side infrastructure.
* The server is responsible for processing incoming requests, interacting with the database, and returning the appropriate responses to the client. 
* The MemoryVault application uses PostgresDB as the database to store stories. The database schema consists of three tables - 'users', 'myvault' and 'roles'    The 'users' table stores information about registered users, while the myvault table stores information about stories created by users then roles tables that store information about the roles of users. 
* The database is accessed using the mysql library, which provides a high-level API for interacting with MysqlDB.  The application provides user authentication and authorization functionality using spring security. When a user logs in or registers, a session ID is generated and stored in the browser's local storage. 
* The application uses bcrypt to hash user passwords before storing them in the database. This ensures that user passwords are never stored in plain text and are always encrypted. 
* The server-side code is structured using the Model-View-Controller (MVC) design pattern. The 'models' folder contains entities for the 'users' and ‘todo’ tables. The 'views' folder contains HTML templates for rendering dynamic views on the client side. The 'controllers' folder contains the business logic for handling incoming requests and returning appropriate responses.  
#### Endpoints links: The following RESTful API endpoints are used by the MemoryVault application: 
1. localhost: 8083/home – accessing homepage               
2. localhost: 8083/services – accessing myvault services  page                                                                                           
3. localhost: 8083/about - accessing about us  page             
4. localhost: 8083/contact - accessing contact us page              
5. localhost: 8083/userhome – accessing homepage of user after successfully log in                                                         
6. localhost: 8083/new - Registers a new user localhost: 8083/login - login a new user                
7. localhost: 8083/registration - Registering a new user   


# Conclusion:
In conclusion, the MemoryVault application is a simple and intuitive note-taking application that provides basic CRUD functionality for stories. It is built using modern web development technologies such as java, spring framework and PostgresDB. The application is designed to be scalable and extensible, allowing for easy addition of new features and enhancements.
