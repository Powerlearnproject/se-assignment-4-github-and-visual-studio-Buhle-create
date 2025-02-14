[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/GvXCZgfk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15350204&assignment_repo_type=AssignmentRepo)
# SE-Assignment-4
Assignment: GitHub and Visual Studio
Instructions:
Answer the following questions based on your understanding of GitHub and Visual Studio. Provide detailed explanations and examples where appropriate.

Questions:
Introduction to GitHub:

What is GitHub, and what are its primary functions and features? Explain how it supports collaborative software development.
1. GitHub is " an online software development platform."(HubSpot Blog, April 2024) It's main features are storing, tracking and collaborating on software projects.Sharing code files and collaboration becomes easier with other developers on open source projects.

Repositories on GitHub:

What is a GitHub repository? Describe how to create a new repository and the essential elements that should be included in it.
Version Control with Git:
2. A GitHub repository is a storage space where project files are managed and stored using Git version control. When creating a new repository, the following steps are taken:
- Sign in to your GitHub account.
- Click on the + icon in the upper right corner and select new repository.
- Add repository details such as the repository name, add a description, choose whether it will be public or private, add a Readme file and choose a license.
- Click the  create repository button then it's done  

Explain the concept of version control in the context of Git. How does GitHub enhance version control for developers?

3. A version control is a system that keep tracks of changes to files over time. GitHub provides a channel that hosts Git repositories, enables collaboration through pull requests, issue tracking, project management tools and integrated CI/CD pipelines.

Branching and Merging in GitHub:

What are branches in GitHub, and why are they important? Describe the process of creating a branch, making changes, and merging it back into the main branch.
4. Branches are separate lines  of development that allows developers to work on features independently from the main code base.When creating a branch, steps taken are as follows: 
-  Clone your repository to your machine.
- Create a new branch.
- Make changes to the code.
- Commit the changes to the branch.
- Push the branch to GitHub.
When merging a branch:
- Switch back to the main branch.
- Merge the changes from the feature branch.
- Push the updated main branch to GitHub.

Pull Requests and Code Reviews:

What is a pull request in GitHub, and how does it facilitate code reviews and collaboration? Outline the steps to create and review a pull request.
5. A pull request is a request to combine changes from one branch into another. Team members can review changes before they are merged. 
 STEPS TO CREATE AND REVIEW A PULL REQUEST:
- Push your branch to GitHub.
- Navigate to the repository on GitHub and press Compare & pull request.
- Fill out PR forms detailing the changes.
- Click create pull request.
REVIEWING A PULL REQUEST:
- Navigate to the repo and click on the pull request button.
- Select the pull request to be reviewed.
- Review the changes, and comments and request changes if necessary.
- Approve and merge if everything is up to date.

GitHub Actions:

Explain what GitHub Actions are and how they can be used to automate workflows. Provide an example of a simple CI/CD pipeline using GitHub Actions.
6. GitHub Actions is a CI/CD service that permits one to automate workflows.
EXAMPLE OF A SIMPLE CI/CD PIPELINE:
name: CI/CD Pipeline
on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v2
    - name: Set up Node.js
      uses: actions/setup-node@v2
      with:
        node-version: '14'
    - run: npm install
    - run: npm test
    - run: npm build
Introduction to Visual Studio:

What is Visual Studio, and what are its key features? How does it differ from Visual Studio Code?
Integrating GitHub with Visual Studio:
7. Visual Studio is an integrated development environment (IDE) for building applications across different platforms. Key features are: - advanced debugging, intelliSense, and merged Git tools. It is different from VS Code which is a lighter version code editor.

Describe the steps to integrate a GitHub repository with Visual Studio. How does this integration enhance the development workflow?

- When integrating GitHub with Visual Studio, 
- Install Git in your system.
- Clone the repository on the Team Explorer.
- Commit and push changes to the GitHub.

Debugging in Visual Studio:

Explain the debugging tools available in Visual Studio. How can developers use these tools to identify and fix issues in their code?
Collaborative Development using GitHub and Visual Studio:
 8. DEBUGGING TOOLS IN VISUAL STUDIO:
 - Breakpoints- Pause execution at certain points
 - Watch Windows- Monitors variable values
 - Call Stack- It views the stack of function cells
 - Immediate Window- Executes code during debugging
 - Developers can use the above tools to identify and fix issues stepping through code, inspecting variables,and analyzing the flow of execution. 

Discuss how GitHub and Visual Studio can be used together to support collaborative development. Provide a real-world example of a project that benefits from this integration-:
- GitHub and Visual Studio can be easily joined to enhance collaborative development. This combination offers different benefits such as version control ,code review,continuous integration and advanced debugging.
The integration benefits are as follows:
- GitHub hosts repos, tracks changes and supports branching and merging. Visual Studio provides a user friendly interface to commit, push, pull and manage branches.
- GitHub facilitates pull requests, code reviews and discussions. Visual Studio permits inline commenting and review capabilities directly from the IDE.

EXAMPLE:
A team of developers is building a web-based Fitness tracker application. The team includes front-end developers, back-end developers, and a project manager.
Repository Setup:The project manager creates a repository on GitHub named expense-tracker.Initializes the repository with a README.md, .gitignore, and license file.
- Cloning and Setting Up the Project:Developers clone the repository to their local machines using Visual Studio.Navigate to Team Explorer > Clone and enter the repository URL.
- Branching Strategy:The team follows a GitFlow workflow, creating branches for features, fixes, and releases.Front-end developers work on a feature/frontend branch, while back-end developers work on feature/backend.
- Development and Commit:Developers write and commit code using Visual Studio’s integrated Git tools.Regular commits are made to keep track of changes and progress.
- Code Reviews and Pull Requests:When a feature is complete, developers push their branch to GitHub and open a pull request.Team members review the pull request, add comments, and suggest changes.Visual Studio displays pull request notifications and allows inline commenting.
- Continuous Integration:GitHub Actions are configured to run automated tests on each pull request.Visual Studio integrates with these actions, allowing developers to see the status of their builds and tests.
- Merging:Once the pull request is approved, it is merged into the main branch.Visual Studio updates the local repository to reflect these changes.
- Deployment:GitHub Actions are used to deploy the application to a staging server upon merging to main.Visual Studio can trigger and monitor these deployments.

REFERENCES:
- geeksforgeeks.org
- HubSpot Blog
- TechTarget.com


Submission Guidelines:
Your answers should be well-structured, concise, and to the point.
Provide real-world examples or case studies wherever possible.
Cite any references or sources you use in your answers.
Submit your completed assignment by [due date].
