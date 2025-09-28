🛍️ AutomationExercise API Testing Project
This repository contains the Postman Collection and supporting files for testing the AutomationExercise E-commerce API. This project demonstrates API testing skills, including request chaining, data-driven testing, and comprehensive test script assertions.

⚙️ Prerequisites
To run these tests locally, you'll need:

Postman Desktop Application: Used to import and execute the collection.

API Backend: This collection is designed to run against the live AutomationExercise API (which is publicly available) or your own locally hosted version of it.

🚀 Getting Started with Postman
1. Project Files
Locate and ensure you have the following file(s) from this repository:

File Name	Type	Purpose
AutomationExercise API Tests.json	Postman Collection	Contains all 14 API requests and associated test scripts.
AutomationExercise.postman_environment.json	Postman Environment	Contains variables like the base URL for the API. (If you have one, otherwise omit this section).

Export to Sheets
2. Import Files into Postman
Open the Postman desktop application.

Click the "Import" button in the top left corner.

Select and upload the AutomationExercise API Tests.json file.

(If applicable) Import the environment file: AutomationExercise.postman_environment.json.

3. Select the Environment
If an Environment file was provided and imported:

In the top-right corner of Postman, use the environment dropdown menu to select the AutomationExercise environment.

Go to the Environments tab on the left sidebar to confirm that the baseUrl or url variable is correctly set (e.g., https://automationexercise.com/api).

4. Collection Structure Overview
The requests are logically organized into folders:

Folder	Description	Key Requests Included
Products	Requests for fetching and searching product data.	GET All Products List, POST Search Product
Brands	Requests for fetching brand data.	GET All Brands List
User	CRUD operations for user accounts, demonstrating request chaining.	POST Create/Register User, PUT Update User, GET User Account Detail
Auth	Requests for user login and verification.	POST Verify Login with Valid/Invalid Details

Export to Sheets
🧪 Running the Tests
To execute all tests and see a comprehensive report:

Select the AutomationExercise API Tests collection in the left sidebar.

Click the "Run" button located on the collection's main tab.

In the Collection Runner window:

Ensure the AutomationExercise environment is selected (if applicable).

Ensure all requests are checked to run.

Click "Run AutomationExercise API Tests".

Expected Outcome
The Postman Runner should execute all requests. Successful requests will show a "Pass" status for all associated tests, demonstrating:

Status Code Validation (e.g., 200 OK, 201 Created).

Response Schema Validation (ensuring the JSON structure is correct).

Data Validation (checking specific values returned in the response).

Variable Usage (e.g., extracting a User ID from a registration response and using it for subsequent update/delete requests).

📞 Contact
For any questions about the collection, test design, or my approach to API testing:

Name: [Your Name]

GitHub: [Link to your GitHub Profile]

Email: [Your Email Address]
