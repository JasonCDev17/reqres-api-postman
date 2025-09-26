Project Overview

This project demonstrates API testing using Postman on the public ReqRes API
.
It covers CRUD operations: GET, POST, PUT, DELETE.
All tests are documented and verified, with bug reports logged in Jira where issues were found.

 Tools & Technologies Used

API Testing Tool: Postman

API Under Test: ReqRes (https://reqres.in/
)

Bug Tracking: Jira (screenshots included)

Test Documentation: Excel / Google Sheets for test cases & RTM


Project Deliverables

Postman Collection → ReqRes_API_Collection.json

Test Cases → Documented CRUD scenarios

Requirements Traceability Matrix (RTM) → Mapping API endpoints to test cases

Bug Reports → Issues logged in Jira with screenshots

Screenshots → Response evidence for all API calls

Endpoints Tested

GET:

List Users

Single User

Single User Not Found

Single Resource

POST:

Create User

PUT:

Update User

DELETE:

Delete User

How to Use

Download or clone this repo:

git clone https://github.com/JasonCDev17/reqres-api-testing.git


Import ReqRes_API_Collection.json into Postman.

Run API requests and verify responses.

Compare results with documented test cases & RTM.

Check bug reports in BugReports/.

Bug Report Example
BUG-API-001 – PUT User Update Returns Incorrect Status

Severity: Medium
Priority: High

 Description

Updating a user via PUT endpoint returns a 200 OK but the response body does not reflect the updated data.

Steps to Reproduce

Send PUT request to /api/users/2

Update "name" and "job" fields

Inspect response body

 Expected Result

Response body should contain updated "name" and "job".

 Actual Result

Response body does not show updated fields.

 Evidence

Areas of Improvement:

-Automation with Newman/CI Integration → Currently, tests are manual in Postman. Integrating with Newman and CI/CD (e.g., GitHub Actions, Jenkins) would enable automated execution.

-Comprehensive Validation → Expand test assertions to include schema validation, response headers, and negative test scenarios.

-Data-Driven Testing → Implement parameterization (e.g., CSV/JSON test data) for scalability and better coverage.

-Enhanced Reporting → Use HTML/Allure reports for clear visualization of test runs, instead of only screenshots.

-Environment & Variable Management → Introduce multiple environments (dev, staging, prod) with global variables for better flexibility.

 What I Have Learned:

-API Testing Fundamentals → Gained hands-on experience with CRUD operations (GET, POST, PUT, DELETE) using Postman.

-Defect Tracking with Jira → Learned how to log, document, and track API-related bugs with evidence.

-Test Documentation → Improved skills in creating test cases and an RTM to ensure endpoint coverage.

-Practical Debugging → Identified discrepancies (e.g., PUT response mismatch), which enhanced problem-solving and attention to detail.

-Collaboration Workflow → Understood how to structure deliverables (collections, RTM, bug reports) for team and stakeholder review.




Endpoints Overview

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | [https://reqres.in/api/users/2](https://reqres.in/api/users/2) | Retrieve user with ID 2 |
| GET    | [https://reqres.in/api/users?page=2](https://reqres.in/api/users?page=2) | Retrieve second page of users |
| GET    | [https://reqres.in/api/users/23](https://reqres.in/api/users/23) | Attempt to retrieve non-existing user |
| GET    | [https://reqres.in/api/unknown/2](https://reqres.in/api/unknown/2) | Retrieve resource with ID 2 |
| POST   | [https://reqres.in/api/users](https://reqres.in/api/users) | Create a new user |
| PUT    | [https://reqres.in/api/users/2](https://reqres.in/api/users/2) | Update user with ID 2 |
| DELETE | [https://reqres.in/api/users/2](https://reqres.in/api/users/2) | Delete user with ID 2 |



 How to Run

1. Clone or download this repository.  
2. Open Postman → click Import → File → Select `Reqres-API.postman_collection.json`.  
3. The collection will appear in Postman.  
4. Click Send** on any request to execute it.  

 Note: Reqres is a demo API, so POST/PUT/DELETE requests simulate changes but do not persist data.

