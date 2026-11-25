![Postman API Tests](https://github.com/dilalwan/postman-api-testing-framework/actions/workflows/postman-api-tests.yml/badge.svg)

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


<img width="532" height="443" alt="image" src="https://github.com/user-attachments/assets/dbffc320-5a0f-4871-90d1-3ff1e5ad0d97" />


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

## 10. CI/CD Integration – GitHub Actions

This project is integrated with GitHub Actions to automatically execute the Postman API testing collection.

### Workflow Triggers

The workflow is configured to run automatically on:

- Push to the `main` branch
- Pull requests targeting the `main` branch
- Manual execution through GitHub Actions (`workflow_dispatch`)

### CI Execution Process

1. GitHub Actions checks out the repository.
2. Postman CLI is installed and configured.
3. The Postman collection is executed.
4. API requests are sent to the Restful Booker public API.
5. JavaScript assertions validate API responses.
6. GitHub Actions reports the execution status as Success or Failure.

### CI Workflow

`GitHub Push / Pull Request` → `GitHub Actions` → `Checkout Repository` → `Postman CLI` → `Execute Collection` → `Assertions` → `CI Result`

### Workflow File

The CI/CD configuration is maintained at:

`.github/workflows/postman-api-tests.yml`

### CI Execution Result

The collection has been successfully executed through GitHub Actions, validating the integration of the Postman API testing collection with the CI pipeline.

This demonstrates automated API test execution as part of a CI workflow.
## 11. Disclaimer

This is an independent learning and portfolio project using a publicly available demonstration API. It is not associated with Vodafone Idea or any production customer billing system.
