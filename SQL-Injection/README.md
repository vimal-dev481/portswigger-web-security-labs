# Vulnerability: SQL Injection (Authentication Bypass)

## Description
The login functionality is vulnerable to SQL Injection.

## Steps to Reproduce
1. Intercept login request using Burp Suite.
2. Modify the username parameter with payload: ' OR 1=1--
3. Forward the request.

## Result
Login successful without valid credentials.

## Impact
An attacker can bypass authentication and access user accounts.

## Recommendation
Use parameterized queries and proper input validation.

