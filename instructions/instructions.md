# 19: Tech Quiz Test Suite

## Your Task

This week, you'll take the starter codebase of a fully functioning Tech Quiz application and enhance it by adding Cypress for both component and end-to-end tests. The app was built using the MERN stack with a React front end, MongoDB database, and Node.js/Express.js server and API. It allows users to take a quiz of ten random questions and view their final score.

To complete the assignment, you'll need to do the following:

1. Install Cypress as a dev dependency.

2. Configure Cypress for both component and end-to-end testing.

3. Create a component test for the quiz component.
   
4. Create an end-to-test for the quiz component.

5. Bonus: Deploy your application to Render with a MongoDB database using MongoDB Atlas. Use the [Deploy with Render and MongoDB Atlas](https://coding-boot-camp.github.io/full-stack/mongodb/deploy-with-render-and-mongodb-atlas) walkthrough for instructions.

## User Story

```md
AS AN aspiring developer
I WANT to take a tech quiz
SO THAT I can test my knowledge and improve my skills
```

## Acceptance Criteria

```md
GIVEN I am taking a tech quiz
WHEN I click the start button
THEN the quiz starts and I am presented with a question
WHEN I answer a question
THEN I am presented with another question
WHEN all questions are answered
THEN the quiz is over
WHEN the quiz is over
THEN I can view my score
WHEN the quiz is over
THEN I can start a new quiz
```

## Mock-Up

The following animation demonstrates the application functionality:

![Animation shows "star wars" typed into a search box and books about Star Wars appearing as results.](./Assets/18-mern-homework-demo-01.gif)

## Getting Started

In order for this application to use a GraphQL API, you’ll need to refactor the API to use GraphQL on the back end and add some functionality to the front end. The following sections contain details about the files you’ll need to modify on the back and front end.

**Important**: You won't need to modify code for the existing application. In this challenge, you'll only be creating tests for the existing application.

Your testing should use CypressLinks to an external site. to run both the component tests and the end-to-end tests. The testing will be invoked using the following command:

```md
npm run test
```

It's recommended that you start with a directory structure that looks like the following example:

```md
├── client/                   // the client application
│    └── client files...    
│  
├── cypress/                  // Folder for Cypress  
│    ├── component/           // Folder for component tests  
│    │    └── Quiz.cy.jsx     // Component tests for the Quiz component  
│    ├── e2e/                 // Folder for end-to-end tests  
│    │    └── quiz.cy.js      // End-to-end tests for the Tech Quiz  
│    ├── fixtures/            // Folder for test fixtures  
│    │    └── questions.json  // Mock data for testing  
│    └── tsconfig.json
│  
├── server/                   // the server application
│    └── client files...
│  
├── .gitignore
│  
├── cypress.config.ts         // Runs the application using imports from lib/
│  
├── package.json
│  
├── tsconfig.json
│  
└── README.md                 // App description, link to video, setup and usage instructions         
```

**Important**: The server for this application requires environment variables to function properly. You'll need to rename the `.env.example` file to `.env`.

## Grading Requirements

> **Note:** If a Challenge assignment submission is marked as “0”, it is considered incomplete and will not count toward your graduation requirements. Examples of incomplete submissions include the following:
>
> * A repository that has no code
>
> * A repository that includes a unique name but nothing else
>
> * A repository that includes only a README file but nothing else
>
> * A repository that only includes starter code

This Challenge is graded based on the following criteria:

### Deliverables: 15%

* Your GitHub repository must contain the application code as well as the configuration and tests using Cypress.

### Walkthrough Video: 32%

* A walkthrough video that demonstrates the component and end-to-end tests running and passing must be submitted.
* The README.md file must include a link to the walkthrough video.
* The walkthrough video must show all tests passing from the command line.
* The walkthrough video must demonstrate how a user would invoke the application from the command line.

### Technical Acceptance Criteria: 40%

Your submission should satisfy all of the preceding acceptance criteria in addition to the following:

* You must use the [Cypress package](https://www.npmjs.com/package/cypress)
* The application must have a component test for the quiz component.
* The application must have an end-to-end test for the quiz component.

### Repository Quality: 13%

* Repository has a unique name.

* Repository follows best practices for file structure and naming conventions.

* Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.

* Repository contains multiple descriptive commit messages.

* Your repository contains a high-quality README with a description and a link to your walkthrough video.

## Review

You are required to submit BOTH of the following for review:

* A walkthrough video that demonstrates the functionality of the application and the application successfully passing tests.
* The URL of your GitHub repository, which should have a unique name and include a README describing the project.
