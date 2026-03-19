# employee-api-testing-postman-newman
# Employee REST API Testing using Postman & Newman

## Project Overview

This project showcases a complete API testing workflow for an Employee Management System using **Postman** and **Newman**.

The objective was not just to execute API calls, but to approach the system like a real QA engineer validating functionality, identifying edge cases, and ensuring reliability through both **positive and negative test scenarios**.

From environment setup to automated execution, this project reflects a practical, hands-on understanding of **real-world API testing practices**.

---

## Tools & Technologies

* **Postman** – API request creation & testing
* **Newman** – Command-line execution & reporting
* **JavaScript** – Writing test scripts & assertions
* **GitHub** – Version control & project presentation

---

## API Used

```
https://dummy.restapiexample.com/api/v1
```

---

## Authentication Note

The selected API does not provide authentication or login functionality.
Instead of forcing an artificial implementation, the focus was placed on **accurate and meaningful testing of available features**.

All core functionalities were tested thoroughly through **CRUD operations**, ensuring realistic and relevant QA coverage.

---

## Test Scenarios Covered

### Environment Setup

* Configured a dedicated Postman environment: **TestEnv**
* Managed reusable variables:

  * `base_url`
  * `employee_id`
* Ensured clean and maintainable request structure

---

### Create Employee

* Created multiple employees using POST requests
* Used structured test data
* Dynamically captured `employee_id` for chaining requests

---

### Get Employee Information

* Retrieved employee details using saved ID
* Verified response structure and correctness
* Ensured data consistency with created records

---

### Update Employee Information

* Updated employee attributes (name, salary, age)
* Verified update responses
* Validated API behavior after modification

---

### Delete Employee

* Deleted employee records using ID
* Verified successful deletion
* Performed negative testing (re-delete scenario)

---

### Retrieve Employee List

* Fetched all employees
* Validated response format and data presence
* Ensured API stability under standard queries

---

## Test Case Coverage

* Total Test Cases: **22**
* ✔ Positive Scenarios
* ✔ Negative Scenarios
* ✔ Edge Case Handling
* ✔ Basic Performance Validation

Included:

```
Employee_API_Test_Cases.xlsx
```

---

## Automation with Newman

All API tests were executed via Newman to simulate real-world automation workflows.

### Run Command:

```bash
newman run collection.json -e environment.json -r html --reporter-html-export report.html
```

---

## Test Report

* Generated HTML report using Newman
* Included execution proof via screenshots

Directory:

```
/screenshots/
```

---

## Project Structure

```
employee-api-testing/
│
├── collection.json
├── environment.json
├── Employee_API_Test_Cases.xlsx
├── report.html
├── screenshots/
└── README.md
```

---

## Key Highlights

* ✔ Complete end-to-end CRUD testing
* ✔ Dynamic data handling using environment variables
* ✔ Automated validation using test scripts
* ✔ Inclusion of negative and edge test cases
* ✔ Clean, structured, and professional documentation

---

## Conclusion

This project reflects a practical understanding of:

* API testing fundamentals
* Test case design and validation logic
* Automation using Newman
* Real-world QA workflow and decision-making

Rather than focusing only on execution, the approach emphasizes **clarity, accuracy, and professional testing practices** — aligning closely with industry expectations.

---

## Author

**Mahmuda Islam Rifah**

---

## ⭐ Support

If you found this project helpful or insightful, consider giving it a ⭐ on GitHub!
