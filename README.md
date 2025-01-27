# API-Testing-with-Postman-and-Newman
API Testing 
API Testing with Postman and Newman
This repository contains a Postman collection for testing various API functionalities. The testing process covers multiple scenarios, including verifying API health, user registration, login, profile updates, and more.

Features
Postman Collection: Includes all necessary requests for API testing.
Scenarios Covered:
Verify API health.
Register a new user.
Log in with user credentials.
Update user profile.
Other CRUD operations (e.g., creating, updating, and deleting notes).
Pre-scripted Tests: Includes automated assertions in the Tests tab for validating responses.
Newman Integration: Supports running collections via the command line using Newman and generating HTML reports.
How to Use
1. Import the Postman Collection
Open Postman.
Click on Import in the top left corner.
Select the provided collection file (e.g., API_Testing_Collection.json).
Import it into your Postman workspace.
2. Set Up Environment Variables
Some requests require dynamic values. Set up the following variables in Postman:

base_url: The base URL of the API (e.g., https://practice.expandtesting.com/notes/api).
auth_token: The token received after login.
3. Execute Requests in Postman
Select the desired request from the imported collection.
Click on Send to execute the request.
Review the response and automated tests in the Tests tab.
4. Run the Collection Using Newman
Prerequisites:
[Node.js](https://nodejs.org/): Install Node.js.
Newman: Install Newman globally using the following command:
cmd run (newman run collection2.json -r htmlextra)

Notes
Ensure you have access to the API and the correct credentials.
Newman simplifies running collections in automated pipelines or CI/CD workflows.
