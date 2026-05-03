# Test Cases – API Testing

## Endpoint
GET https://jsonplaceholder.typicode.com/users

---

## TC-01 – Validate status code

**Description:** Verify that the API returns status code 200

**Steps:**
1. Send GET request to /users

**Expected Result:**
- Status code should be 200

---

## TC-02 – Validate response time

**Description:** Verify that the API response time is acceptable

**Steps:**
1. Send GET request to /users

**Expected Result:**
- Response time should be less than 500ms

---

## TC-03 – Validate response is not empty

**Description:** Verify that the API returns a list of users

**Steps:**
1. Send GET request to /users

**Expected Result:**
- Response should contain at least 1 user

---

## TC-04 – Validate required fields

**Description:** Verify that user object contains required fields

**Steps:**
1. Send GET request
2. Check first user object

**Expected Result:**
- Fields present:
  - id
  - name
  - username
  - email

---

## TC-05 – Validate data types

**Description:** Verify that fields have correct data types

**Steps:**
1. Send GET request
2. Check first user

**Expected Result:**
- id should be a number
- email should be a string

---

## TC-06 – Validate email format

**Description:** Verify that email field contains "@"

**Steps:**
1. Send GET request
2. Check email field

**Expected Result:**
- Email should contain "@"

---

## TC-07 – Validate minimum number of users

**Description:** Verify that API returns multiple users

**Steps:**
1. Send GET request

**Expected Result:**
- Response should contain more than 5 users

---

## TC-08 – Negative test (invalid endpoint)

**Description:** Verify API behavior when endpoint is incorrect

**Steps:**
1. Send GET request to /userssss

**Expected Result:**
- Status code should be 404