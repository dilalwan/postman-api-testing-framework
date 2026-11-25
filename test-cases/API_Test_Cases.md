# API Test Cases – Booking API Testing Framework

**Project:** Booking API Testing Framework  
**Base URL:** https://restful-booker.herokuapp.com  
**Tool:** Postman  
**API Documentation:** https://restful-booker.herokuapp.com/apidoc/index.html

## 1. Test Scenarios

| Test ID | API / Method | Test Scenario | Expected Result |
|---|---|---|---|
| TC_001 | GET – All Bookings | Retrieve all booking IDs | HTTP 200; response contains booking IDs |
| TC_002 | GET – Booking by ID | Retrieve an existing booking using a valid ID | HTTP 200; booking details are returned |
| TC_003 | GET – Booking by ID | Retrieve booking using an invalid ID | HTTP 404; booking not found |
| TC_004 | POST – Create Booking | Create a booking with valid request data | HTTP 200; booking ID and booking details are returned |
| TC_005 | POST – Create Booking | Create a booking with missing or invalid mandatory fields | Request is rejected or validation behavior matches the API contract |
| TC_006 | POST – Generate Token | Generate authentication token using valid credentials | HTTP 200; token is returned |
| TC_007 | POST – Generate Token | Generate token using invalid credentials | Authentication is rejected |
| TC_008 | PUT – Update Booking | Update an existing booking with valid data and authentication | HTTP 200; booking is updated |
| TC_009 | PUT – Update Booking | Update booking without a valid authentication token | HTTP 401/403; update is rejected |
| TC_010 | PATCH – Update Booking | Partially update an existing booking | HTTP 200; specified fields are updated |
| TC_011 | PATCH – Update Booking | Verify fields not included in the PATCH request remain unchanged | Unspecified fields retain their previous values |
| TC_012 | DELETE – Booking | Delete an existing booking with valid authentication | HTTP 201; deletion is successful |
| TC_013 | GET – Booking by ID | Retrieve a booking after deletion | HTTP 404; deleted booking is no longer available |
| TC_014 | GET – Booking by ID | Verify response contains the expected booking fields and data types | Response structure and data types match the API contract |
| TC_015 | API Validation | Verify response status, headers, response time and JSON structure | All applicable Postman assertions pass |

## 2. Validation Coverage

- HTTP status code validation
- Response body and JSON schema validation
- Mandatory field validation
- Booking ID validation
- Authentication and authorization validation
- Data persistence validation after POST, PUT and PATCH
- Data integrity validation after DELETE
- Negative testing for invalid IDs and credentials
- Response time and header validation

## 3. Execution Summary

| Metric | Result |
|---|---:|
| Total assertions | 27 |
| Passed assertions | 27 |
| Failed assertions | 0 |
| Execution errors | 0 |
| Iterations | 1 |
| Average response time | 341 ms |
| Total execution duration | 12.069 seconds |

*Execution metrics reflect the recorded Postman Collection Runner execution. They are not a claim that all 15 documented scenarios were individually executed.*

## 4. Notes

- This is an independent API testing practice project using the public Restful Booker demo API.
- Test results may vary because the demo service is shared and its data can change.
- No production or Vodafone Idea systems are involved.
