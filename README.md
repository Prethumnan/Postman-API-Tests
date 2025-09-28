# 🛍️ AutomationExercise API Testing Project

This repository showcases API testing skills using Postman for the AutomationExercise E-commerce API. This project demonstrates key testing concepts, including sequential request execution, data-driven workflows, and comprehensive test script assertions.

---

## ⚙️ Prerequisites

To successfully run these tests, you must have the following installed:

1.  **Postman Desktop Application:** Used to import and execute the collection.

*(Note: This collection is designed to run against the publically available AutomationExercise API, so no backend setup is typically required.)*

---

## 🚀 Getting Started with Postman

### 1. Locate Project Files

Ensure you have the following file(s) from this repository:

| File Name | Type | Purpose |
| :--- | :--- | :--- |
| **`AutomationExercise API Tests.json`** | Postman Collection | Contains all 14 API requests and associated test scripts. |
| **`AutomationExercise.postman_environment.json`** | Postman Environment (Optional) | Contains essential variables like the `baseUrl`. |

### 2. Import Files into Postman

1.  Open the **Postman** desktop application.
2.  Click the **"Import"** button in the top left corner.
3.  Select and upload the **`AutomationExercise API Tests.json`** file.
4.  If an Environment file is provided, import the **`AutomationExercise.postman_environment.json`** as well.

### 3. Configure the Environment (Crucial Step)

If an environment file was imported:

1.  In the top-right corner of Postman, use the environment dropdown menu to select the **`AutomationExercise`** environment.
2.  Go to the **Environments** tab on the left sidebar.
3.  Confirm that the base URL variable (e.g., `baseUrl` or `url`) is correctly set to the API endpoint (e.g., `https://automationexercise.com/api`).
    * **Always check for sensitive data:** Ensure any API keys, passwords, or tokens are set in the **Current Value** field and **not** the Initial Value.

---

## 🗂️ Collection Structure

The requests are logically grouped into folders to ensure a clear and maintainable test structure:

| Folder | Description | Key Requests Included (Examples) |
| :--- | :--- | :--- |
| **Products** | Requests for fetching all products and performing product searches. | `GET All Products List`, `POST Search Product` |
| **Brands** | Requests for retrieving brand-related data. | `GET All Brands List` |
| **User** | **Critical workflow for User CRUD operations.** Requests here often rely on variables set in previous requests. | `POST Create/Register User`, `PUT Update User`, `DELETE User Account` |
| **Auth** | Requests for authenticating and validating user credentials. | `POST Verify Login with Valid/Invalid Details` |

---

## 🧪 Running the Tests

To execute the entire test suite and generate a report:

1.  Select the **`AutomationExercise API Tests`** collection in the left sidebar.
2.  Click the **"Run"** button located on the collection's main tab.
3.  In the Collection Runner window:
    * Ensure the correct **`AutomationExercise`** environment is selected.
    * Verify that all requests are selected for execution.
    * **Run Order:** The requests are ordered to execute a complete flow (e.g., Register then Update then Delete), which is critical for successful testing.
4.  Click **"Run AutomationExercise API Tests"**.

### Test Assertions Demonstrated

Upon completion, the Postman Runner report will show detailed results confirming:

* **Status Code Validation** (e.g., HTTP 200 OK, 201 Created).
* **Response Body Schema Validation** (ensuring data integrity).
* **Data Consistency** (checking specific values, such as 'message' or 'responseCode').
* **Sequential Execution Success** (passing data/tokens between requests via variables).

---

## 🤝 Contact

Feel free to reach out with any questions regarding this API testing project or the methodologies used.

* **Name:** Prethumnan
* **GitHub:** https://github.com/Prethumnan
* **Email:** prethumnan77@gmail.com
