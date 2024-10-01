## 🧪 Microservices API Testing Collection
This repository contains various Postman collections designed to help you perform thorough testing of microservices through Contract Testing, Integration Testing, Mock Data Generation, Performance Testing, and Regression Testing. Each collection focuses on different aspects of microservices testing, ensuring robust and resilient API behavior.

## 📂 Collections Overview
## 1. Contract Testing
About this Collection
Contract tests ensure that two separate systems can communicate effectively by validating the compatibility between APIs. This collection helps you ensure that your APIs and their consumers are following the defined contract.

Using the Collection:

Step 1: Send the sample requests and review the response and test results.
Step 2: Replace the sample request URLs with your API endpoints.
Step 3: Customize the tests in the "Tests" tab as needed. Save your changes after modification.

## 2. Integration Testing
About this Collection
Integration testing ensures that different components of your API function together seamlessly. This collection tests the integration of multiple endpoints in a workflow, such as registering a token, fetching a unique generated name, and unregistering the token.

Tested Endpoints:

POST /register
POST /unregister
GET /my-name
Using the Collection:

Set up the requests in the order of the operation.
Validate that the flow of data between endpoints works as expected.
Ensure that data persists correctly between requests.

## 3. Mock Data Generation
About this Collection
Postman provides dynamic variables, powered by the Faker library, to generate randomized sample data. This collection showcases how you can use dynamic variables to create mock data, simulating real-world data in API testing.

Using the Collection:

Step 1: Select and send requests.
Step 2: Review the request "Body" and "Pre-request Script" tabs to understand how dynamic variables generate mock data.
Step 3: Customize dynamic variables based on your use case. Save changes and send requests.
Step 4: Analyze the responses to see generated mock data (responses differ each time due to randomization).

## 4. Performance Testing
About this Collection
This collection allows you to test the performance of your API by simulating varying sizes of query parameters. Performance tests help identify bottlenecks and optimize the performance of your API under different load conditions.

Using the Collection:

Step 1: Replace placeholder URLs and parameters with your API’s base URL and query parameters.
Step 2: (Optional) Modify the size of query parameters to better reflect your specific use case.
Step 3: Run the collection using Postman’s Collection Runner or Newman CLI.
Step 4: Analyze the results to detect bottlenecks, slow response times, and potential performance issues.

## 5. Regression Testing
About this Collection
Regression testing ensures that your API functions as expected after updates or changes. This collection includes tests for status code verification, JSON schema validation, response time checks, response body structure, and header verification.

Tests Included:

Status Code Verification: Verify that the API returns the correct status codes for different requests.
JSON Schema Verification: Ensure the API response follows the defined JSON Schema.
Response Time Verification: Ensure API response times are within the acceptable range.
Response Body Verification: Validate the structure and content of the response.
Header Verification: Confirm that the correct headers are present and valid.
Using the Collection:

Step 1: Send the sample requests and check the responses and test results.
Step 2: Replace the sample URLs with your API’s endpoints.
Step 3: Customize the tests as necessary. Save your changes.
Step 4: Run the collection by selecting "Run."


## 🚀 How to Use
1. Clone the Repository:
git clone https://github.com/RahulKumar208/Microservices-Testing-with-Postman.git

2. Import the Postman Collection:

Open Postman, and click on Import.
Select the relevant Postman collection from this repository (Contract Testing, Integration Testing, etc.).

3. Set Up Your Environment:

Define your API base URL and other relevant environment variables (if required) in Postman.
Customize the requests and tests based on your API setup.

4. Run the Collections:

Use Postman’s Collection Runner to execute the tests for a full suite run.
Optionally, use Newman (Postman’s CLI tool) for continuous integration (CI) pipelines.

5. Analyze the Results:

Review the test results for response validation, performance metrics, and error checks.

## 🛠️ Tools and Technologies
Postman: API testing tool.
ChaiJS: JavaScript assertion library used in Postman’s test scripts.
Faker.js: Library for generating dynamic mock data.
Newman: Command-line tool to run Postman collections.
