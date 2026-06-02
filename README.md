# API Security Risk Analysis – Future Interns Task 3 (2026)

## Overview

This project contains an API Security Risk Analysis conducted as part of the Future Interns Cyber Security Internship Task 3.

The assessment was performed on the JSONPlaceholder public testing API using Postman on Kali Linux. The objective was to identify common API security risks through read-only testing and documentation review while following ethical security practices.

---

## Objective

The goal of this task was to:

* Analyze a public API
* Review authentication and authorization controls
* Identify common API security risks
* Assess potential business impact
* Provide remediation recommendations
* Document findings in a professional security report

---

## Target API

JSONPlaceholder Test API

https://jsonplaceholder.typicode.com

---

## Tools Used

* Kali Linux Virtual Machine
* Postman
* Git & GitHub
* Web Browser

---

## Testing Methodology

1. Reviewed API documentation.
2. Tested publicly available endpoints.
3. Inspected API responses and headers.
4. Evaluated authentication requirements.
5. Analyzed authorization controls.
6. Assessed data exposure risks.
7. Documented findings and recommendations.

---

## API Endpoints Tested

* GET /users
* GET /users/1
* GET /users/2

---

## Key Findings

### 1. Unauthenticated Access

**Severity:** Medium

The API allows access to user information without requiring authentication.

### 2. Excessive Data Exposure

**Severity:** Medium

User responses expose detailed information including email addresses, phone numbers, company information, and location details.

### 3. Potential Broken Object Level Authorization (BOLA)

**Severity:** High

User information can be accessed by changing object identifiers in the request URL. In a real-world application, this could result in unauthorized access to other users' data.

---

## Risk Summary

| Finding                 | Severity |
| ----------------------- | -------- |
| Unauthenticated Access  | Medium   |
| Excessive Data Exposure | Medium   |
| Potential BOLA          | High     |

---

## Recommendations

* Implement strong authentication mechanisms.
* Enforce authorization checks for every request.
* Apply Role-Based Access Control (RBAC).
* Reduce unnecessary data exposure.
* Monitor and log API activity.
* Follow OWASP API Security Top 10 guidelines.

---

## Repository Structure

```text
FutureInterns_API_Security_Task3
├── report
│   └── API_Security_Risk_Analysis_Report.pdf
├── screenshots
│   ├── users_endpoint.png
│   ├── bola_user1.png
│   └── bola_user2.png
├── notes
│   ├── api_endpoints_tested.txt
│   ├── findings.txt
│   └── methodology.txt
└── README.md
```

---

## Ethical Notice

This assessment was performed on a publicly available testing API intended for educational and development purposes. No exploitation attempts, denial-of-service testing, or unauthorized activities were conducted.

---

## Author

**SHARRUN**

Future Interns – Cyber Security Internship Program (2026)
