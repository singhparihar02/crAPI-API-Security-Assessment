# crAPI – API Security Assessment

Hands-on API security assessment of **OWASP crAPI (Complete Ridiculous API)** using Burp Suite and a locally deployed Docker environment.

## Project Overview

This project documents practical API security testing performed against OWASP crAPI, an intentionally vulnerable application designed for learning and practising API security.

The assessment focused on identifying authentication, authorization, injection, information exposure, and other API security weaknesses.

## Lab Environment

| Component | Details |
|---|---|
| Target Application | OWASP crAPI |
| Deployment | Local Docker environment |
| Interception and Testing | Burp Suite Community Edition |
| JWT Testing | Burp Suite JWT Editor extension |
| Application Access | Localhost |

## Security Testing Coverage

The assessment covered the following areas:

- Broken Object-Level Authorization (BOLA / IDOR)
- Broken User Authentication
- Excessive Data Exposure
- Lack of Resource and Rate Limiting
- Broken Function-Level Authorization (BFLA)
- Mass Assignment
- Injection (SQL and NoSQL)
- Broken Access Control
- JWT Security Testing:
  - Algorithm Confusion (RS256 to HS256)
  - `none` Algorithm Acceptance
  - JWT Signature Validation

## Tools Used

- **Burp Suite Community Edition:** Request interception, analysis, and manual API security testing.
- **Burp Suite JWT Editor:** JWT inspection and manipulation.
- **Docker Desktop:** Local deployment and management of the crAPI lab.

## Testing Methodology

1. Deployed the crAPI application locally using Docker Desktop.
2. Explored application functionality and identified API requests.
3. Intercepted and analysed HTTP requests and responses using Burp Suite.
4. Modified request parameters, headers, HTTP methods, and authentication tokens.
5. Tested authorization boundaries, authentication mechanisms, input validation, and API behavior.
6. Documented observations, proof-of-concept evidence, security impact, and remediation recommendations.

## Assessment Report

The detailed assessment report contains testing observations, request/response evidence, proof-of-concept screenshots, and remediation recommendations.

**Report:** `Assessment-Report/crAPI-Security-Assessment-Report.pdf`

## Key Learning Outcomes

- Understanding API authentication and authorization weaknesses.
- Identifying BOLA, IDOR, and privilege escalation issues.
- Testing rate-limiting and resource-consumption controls.
- Analysing SQL and NoSQL injection scenarios.
- Understanding JWT structure and common JWT attack techniques.
- Using Burp Suite for manual API security testing.
- Documenting vulnerabilities and recommending security improvements.

## Disclaimer

This project was conducted in a controlled local lab environment using an intentionally vulnerable application for educational purposes.

All testing was performed for learning and authorized security assessment practice.
