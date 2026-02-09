QA Test Plan – Weather API Portfolio

**1. Objective**

The objective of this test plan is to validate the functionality, reliability, and error handling of the Weather API used for QA portfolio demonstration.

This project demonstrates:
1. API functional testing
2. Positive and negative scenario validation
3. Postman test scripting
4. Bug reporting
5. Test documentation and reporting
6. Version control using Git

**2. Scope**

**In Scope**
Weather API current weather endpoint testing
Response validation (status codes, JSON structure, data types)
Authentication and API key validation
Error handling scenarios
POST and PUT requests using public test API (JSONPlaceholder)
Test documentation and reporting

**Out of Scope**
Performance/load testing
Security penetration testing
UI testing
Database validation (no DB access available)

**3. Test Approach**
Testing is performed using **manual API testing** with automated validation scripts in **Postman**.

Types of testing performed:
1. Functional testing
2. Negative testing
3. Input validation
4. Response schema validation
5. Status code verification
6. Data type validation

**Scenario coverage:**

Valid requests
Invalid city names
Missing parameters
Invalid authentication
Edge cases (long strings, special characters)

**4. Tools Used**
**Tool	  **              **   Purpose**
Postman	                 API testing and automation scripts
Newman	                 Collection execution and HTML reports
Jira	                   Test management and bug tracking
Zephyr	                 Test case management
Git/GitHub	             Version control and portfolio hosting
Excel	                   Test case documentation


**5. Test Environment**

**Component	             Details**
API	                     OpenWeatherMap API
Tool	                   Postman Desktop
OS	                     Any (cross-platform)
Auth	                   API key authentication

**Environment variables used:**
BASE_URL
API_KEY

**6. Test Data**

**Test Type**               **Data Used**
Valid city	                  London, São Paulo
Invalid city	                NoCityHere
Empty input	                  Blank city
Numeric input	                12345
Long string	                  200+ character string
API key tests	                Valid, missing, invalid


**7. Entry & Exit Criteria**

**Entry Criteria**
API endpoints accessible
Postman configured
Environment variables created
Test cases written

**Exit Criteria**
All test cases executed
Results documented
Bugs logged
Test report generated

**8. Deliverables**

Test Plan
Test Cases (Excel)
Postman Collections
Execution Reports
Bug Reports
Git repository with full documentation

**9. Risks & Mitigation**

**Risk**                    	**Mitigation**
Public API downtime	            Retest later / document issue
API key expiration	            Regenerate key
Rate limits	                    Use limited test runs
Data inconsistency	            Validate response structure instead of exact values

**10. Success Criteria**

**Project is considered successful when:**
All planned test cases executed
Positive scenarios return expected data
Negative scenarios return correct errors
Reports and bug documentation completed
