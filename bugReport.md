# Bug Report – API Testing

## Bug ID
BUG-01

## Title
Invalid endpoint returns 404 error

## Description
When sending a request to an incorrect endpoint, the API returns a 404 status code.

## Steps to Reproduce
1. Send GET request to:
   https://jsonplaceholder.typicode.com/userssss

## Expected Result
The API should return an error response indicating that the endpoint is invalid.

## Actual Result
The API returns status code 404.

## Severity
Low

## Priority
Low

## Environment
Postman

## Evidence
![404 Error](evidencias/api-error-404.png)

---

## Bug ID
BUG-02

## Title
API response time could impact performance in real scenarios

## Description
Although the response time is below 500ms, performance should be monitored under high load scenarios.

## Steps to Reproduce
1. Send GET request to:
   https://jsonplaceholder.typicode.com/users

## Expected Result
API should maintain consistent performance under load.

## Actual Result
Response time varies depending on request.

## Severity
Medium

## Priority
Medium

## Environment
Postman

## Evidence
![Response Time](evidencias/api-complete-tests.png)