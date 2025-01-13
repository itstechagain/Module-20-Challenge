# Module-20-Challenge
# Full-Stack CI/CD Application with Cypress Tests

Description

This project focuses on building a CI/CD pipeline for a full-stack app with GitHub Actions and Cypress. 
The idea is to automatically run tests and deploy the app whenever code gets merged into specific branches, helping maintain code quality and keeping the deployment process smooth and hassle-free.

## Table of Contents
- [Features] (#features )
- [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [License](#license)
- [Contributing](#contributing)
- [Questions](#questions)
- [Demo](#demo)

## Features
Integration with Cypress tests triggered by Pull Requests to the develop branch.
Continuous Deployment to Render triggered when changes are merged from develop to the main branch.
Full-stack MERN application with a user-friendly interface.

## Installation
Clone this repository to your local machine:
git clone https://github.com/yourusername/Module-20-Challenge

Navigate to the project directory:
cd Module-20-Challenge

Install the required dependencies:
npm install

Configure the required environment variables:
Create a .env file and add your MongoDB URI and necessary keys.

## Usage
npm start
Open your browser and navigate to http://localhost:3001
Use the application

CI/CD Pipeline:
A GitHub Action is triggered when a Pull Request is made to the development branch.
The action runs Cypress component tests to ensure the code meets quality standards.
If all tests pass, the Pull Request can be merged.

Continuous Deployment:
Once the code is merged to the main branch, another GitHub Action triggers automatic deployment to Render.
The deployment process ensures that the latest version of the application is always live and accessible.

Setup Instructions:
Create a develop branch and ensure all feature branches are merged into it.
Set up GitHub Actions with two separate YAML files:
	One for running Cypress tests on Pull Requests to the develop branch.
	Another for deploying the application to Render when the main branch is updated.

Render Configuration
	Deploy the application to Render and set up MongoDB.
	Navigate to the Render settings and disable Auto-Deploy.
	Copy the Deploy Hook URL and add it to your GitHub repository secrets as RENDER_DEPLOY_HOOK.
	Ensure you have added the Render API Key in the GitHub repository secrets as RENDER_API_KEY.

## Testing

This project uses Cypress for component and end-to-end testing.

Running Tests Locally:

Install Cypress as a dev dependency:
	npm install cypress --save-dev

Run the Cypress Test Runner:
npm run test

Select the test files to execute:

Component Test: Ensures individual components render and function correctly.

End-to-End Test: Simulates user interactions with the entire application.

GitHub Actions Tests:
Cypress tests automatically run on GitHub Actions when a Pull Request is created to the develop branch.
Test results are available directly on the GitHub Actions page.

## License
![License](This project is not licensed).

## Contributing

Contributions are not necessary or currently required

## Questions

For any questions, feel free to reach out:

GitHub: itstechagain

## Demo
Demo Link :