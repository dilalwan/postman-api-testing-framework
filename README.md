# postman-api-testing-framework
REST API testing framework using Postman, JavaScript assertions, CRUD operations, authentication and automated test execution.

# REST API Testing Framework using Postman

## 1. Project Overview

This is an independent REST API testing and automation project developed using Postman and JavaScript.

The project uses the publicly available Restful Booker API to demonstrate API testing concepts, CRUD operations, authentication, positive and negative testing, response validation and automated test execution.

## 2. Tools and Technologies

- Postman
- JavaScript
- REST APIs
- JSON
- GitHub

## 3. API Operations Covered

| HTTP Method | Operation | Description |
|---|---|---|
| GET | Retrieve Bookings | Fetch all bookings and individual booking details |
| POST | Create Booking | Create a new booking |
| PUT | Update Booking | Replace complete booking details |
| PATCH | Partial Update | Update specific booking fields |
| DELETE | Delete Booking | Delete an existing booking |

## 4. Testing Scope

- Positive and negative API testing
- HTTP status code validation
- Request and response validation
- JSON response structure and data type validation
- Authentication and token handling
- Dynamic variables and API chaining
- CRUD operation validation
- Data persistence verification
- JavaScript automated assertions
- End-to-end API workflow testing

## 5. Automation Approach

Postman JavaScript assertions are implemented to validate response status codes, mandatory fields, data types, response values and expected business behaviour.

Dynamic collection variables are used to capture authentication tokens and booking IDs and reuse them across dependent API requests.

The Collection Runner is used to execute the API test suite sequentially and generate execution results.

## 6. Execution Results

Initial collection execution results:

| Metric | Result |
|---|---:|
| Total assertions | 27 |
| Passed | 27 |
| Failed | 0 |
| Errors | 0 |
| Iterations | 1 |
| Average response time | 341 ms |
| Execution duration | 12.069 seconds |

## 7. Repository Structure

- `collections/` – Exported Postman collection
- `reports/` – API test execution report
- `screenshots/` – API request and response evidence
- `test-cases/` – Test scenarios and test cases

## 8. How to Execute

1. Download or clone this repository.
2. Import the Postman collection JSON into Postman.
3. Configure the required collection variables.
4. Generate an authentication token.
5. Open Collection Runner.
6. Execute the requests in the required sequence.
7. Review the test execution results.

## 9. API Documentation

[Restful Booker API Documentation](https://restful-booker.herokuapp.com/apidoc/index.html)

## 10. Disclaimer

This is an independent learning and portfolio project using a publicly available demonstration API. It is not associated with Vodafone Idea or any production customer billing system.
