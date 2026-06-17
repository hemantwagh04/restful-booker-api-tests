# RestfulBooker API Testing Project

## Overview
Complete API testing suite for RestfulBooker (hotel booking API) using Postman. 
Tests cover full CRUD operations with authentication, assertions, and negative testing.

## Technologies Used
- **Postman** - API testing tool
- **RestfulBooker API** - Hotel booking REST API
- **JSON** - Request/response format
- **JavaScript** - Test assertions (pm.test, pm.expect)

## Test Suite Coverage
| Test ID | Endpoint | Method | Scenario | Status |
|---------|----------|--------|----------|--------|
| TC01 | /auth | POST | Create auth token | ✅ 200 |
| TC03 | /booking | POST | Create valid booking | ✅ 200 |
| TC08 | /booking/{id} | GET | Retrieve existing booking | ✅ 200 |
| TC09 | /booking/999999 | GET | Get non-existent booking | ✅ 404 |
| TC11 | /booking/{id} | PUT | Update with valid auth token | ✅ 200 |
| TC14 | /booking/{id} | DELETE | Delete with valid auth token | ✅ 201 |

## Key Features
✅ **Authentication** - Token-based auth with environment variables
✅ **CRUD Operations** - Create, Read, Update, Delete bookings
✅ **Data Chaining** - Uses environment variables to pass data between requests
✅ **Assertions** - Status codes, response body validation, data verification
✅ **Negative Testing** - Tests edge cases (non-existent resources, 404 errors)
✅ **Response Time** - Validates API response times

## Test Results
- **Total Tests:** 16
- **Passed:** 13+ ✅
- **Failed:** 0 ("All negative test cases returned expected error responses — no unexpected failures.")
- **Avg Response Time:** 600ms

## How to Use

### Import into Postman
1. Open Postman
2. Click **Import** → Select `RestfulBooker-API-Tests.postman_collection.json`
3. Import environment: `RestfulBooker-Dev.postman_environment.json`

### Run the Collection
1. Select the collection in left sidebar
2. Click **Run** (top left)
3. All tests will execute in sequence
4. View results in the run summary

## Skills Demonstrated
✅ REST API testing with Postman
✅ Test automation and assertions
✅ API authentication and authorization
✅ CRUD operation testing
✅ Error handling and negative testing
✅ Request/response validation
✅ Environment variable management

## Project Structure
