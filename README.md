# QA Project – API Testing with Postman

## Project Summary

This project demonstrates API testing using Postman, including positive and negative test scenarios. The tests validate response status, performance, data structure, and error handling.

The goal is to simulate real QA activities, ensuring that the API behaves correctly under different conditions.

---

## Business Context

This project simulates the validation of a user management API.

The tested endpoint returns a list of users, and the objective is to verify whether the API provides valid, consistent, and properly structured user data.

The tests were designed to validate successful responses, data integrity, response performance, and error handling.

---

## Test Strategy

The testing strategy includes:

- Functional API testing
- Status code validation
- Response time validation
- JSON structure validation
- Data type validation
- Required field validation
- Negative testing
- Evidence documentation

The goal is to verify both expected behavior and error scenarios.

---

## Tested API

JSONPlaceholder API  
https://jsonplaceholder.typicode.com/

---

## Objective

Perform API testing to validate:

- Response status codes  
- Response time (performance)  
- Data integrity and structure  
- Business rule consistency  
- Error handling (negative scenarios)  

---

## Tools Used

- Postman  
- JSONPlaceholder API  

---

## Test Scenarios

### Positive Test – GET Users

**Endpoint:**

```txt
GET https://jsonplaceholder.typicode.com/users
```

### Validations performed:

- Status code is 200
- Response time is less than 500ms
- Response contains users
- First user has required fields (id, name, username, email)
- First user ID is a number
- First user email contains "@"
- Response has more than 5 users

### Result: 
7/7 tests passed

---

### Negative Test – Invalid Endpoint

**Endpoint:**

```txt
GET https://jsonplaceholder.typicode.com/userssss
```
### Validation performed:

Status code is 404

### Result: 
Test passed (error correctly handled)

---

## Evidence:

### GET Users Request
![GET Users](evidencias/api-get-users.png)

---

### Validations Applied
![Validations](evidencias/api-validations.png)

---

### Complete Test Results (7/7 Passed)
![Complete Tests](evidencias/api-complete-tests.png)

---

### Negative Test – 404 Error
![404 Error](evidencias/api-error-404.png)

---

## Skills Practiced
- API Testing
- Postman
- Manual Testing
- Status Code Validation
- Response Time Analysis
- JSON Data Validation
- Negative Testing
- Test Documentation

---

## Highlights

- Created and executed API test scenarios using Postman
- Implemented automated validation scripts (status, performance, data structure)
- Designed and documented test cases (functional + negative scenarios)
- Reported findings with structured bug reports and visual evidence
- Simulated real QA workflow: planning → execution → validation → reporting

---

## Author

Tainara Lauschner
QA Analyst in training
https://github.com/tainaralauschner