 Reqres API Postman Project

This repository contains a Postman collection for testing the Reqres API.  
The collection includes 4 GET requests, 1 POST, 1 PUT, and 1 DELETE to demonstrate common API interactions.



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

