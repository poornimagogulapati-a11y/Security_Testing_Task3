"Company": CODETECH IT SOLUTIONS

"Name":GOGULAPATI LAKSHMI POORNIMA

"INTERN ID":CTIS5653

"DOMAIN": SOFTWARE TESTING

"DURATION": 4 WEEKS

"MENTOR": NEELA SANTHOSH

PROJECT TITLE: Web Application Security Testing
------------------------------------------------------------

Objective:
To perform manual security testing on a demo banking web application and identify common vulnerabilities such as SQL Injection and Cross-Site Scripting (XSS). The testing was conducted for educational purposes on a legally permitted demo website.

------------------------------------------------------------

TEST CASE 1: SQL INJECTION TEST

Vulnerability Type: SQL Injection
Description: SQL Injection is a vulnerability where attackers inject malicious SQL queries into input fields to manipulate the database.

Test Input:
Username: ' OR '1'='1
Password: ' OR '1'='1

Expected Result:
Application should reject invalid login attempts.

Actual Result:
Application displayed invalid login message and did not allow login bypass.

Status: Not Vulnerable

Screenshot:
![SQL Injection Test](SQLinjectiontest.png)
![SQL Injection Result](SQLtesting_vulnerable.png)

------------------------------------------------------------

TEST CASE 2: CROSS-SITE SCRIPTING (XSS) TEST

Vulnerability Type: Cross-Site Scripting (XSS)
Description: XSS allows attackers to inject malicious scripts into web pages viewed by other users.

Test Input:
<script>alert('XSS')</script>

Expected Result:
Application should block or sanitize script input.

Actual Result:
Alert popup appeared successfully.

Status: Vulnerable

Screenshot:
![XSS Test](XSStest.png)
![XSS Result](XSSresults.png)

------------------------------------------------------------

TEST CASE 3: ACCOUNT ACCESS TESTING

Test Description: Verify secure access to account summary and transaction history pages.

Valid Credentials:
Username: jsmith
Password: demo1234

Test Scenario 1:
Login using valid credentials.

Result:
Login successful and account summary displayed.

Test Scenario 2:
Directly accessing account page without login.

Result:
Application redirected user to login page.

Status: Secure Access Control Implemented

------------------------------------------------------------

Overall Conclusion:
The application is protected against basic SQL Injection attacks.
The application is vulnerable to Cross-Site Scripting (XSS).
Proper input validation and output encoding mechanisms should be implemented to enhance security.
