# Manual-Testing-Project-The-Dummy-Site
> **A complete, structured QA documentation project showcasing real-world manual testing skills — including bug discovery, test case design, and security vulnerability identification.**


👤 Author
Chandan Kumar  
Manual QA Tester | Fresher  
📧 [ck598364@gmail.com]  
🔗 [https://www.linkedin.com/in/chandankumar-cse/]
---
📑 Table of Contents
Project Overview
Objectives
Application Under Test
Testing Methodology
Modules Tested
Test Environment
Test Case Summary Table
Detailed Bug Reports
Working Features (Pass Results)
Defect Summary & Metrics
Risk Analysis
Key Learnings
How to Use This Repository
---


📌 Project Overview
This project documents a complete manual testing cycle performed on "The Dummy Site" — a web application specifically built for testing practice. The goal was to simulate the role of a QA Engineer and evaluate the application's behavior under:
Normal (valid) user inputs
Invalid and unexpected inputs
Edge cases and boundary values
Security-sensitive workflows like OTP verification
Testing covered 8 major modules with a focus on input validation, authentication security, and form workflow integrity.
---

🎯 Objectives
#	Objective
1	Verify whether input validation is correctly implemented across all forms
2	Test system behavior when provided with invalid, special character, or random data
3	Identify functional defects and security-related vulnerabilities
4	Analyze how different modules interact under edge cases
5	Document all findings in a structured, industry-standard QA format
---

🌐 Application Under Test
Detail	Info
App Name	The Dummy Site
Type	Web Application (Testing Practice Platform)
Purpose	QA/Testing Learning & Practice
Testing Type	Manual
---

🧠 Testing Methodology
🔹 Functional Testing
Verifying that each feature/module performs as expected under normal, correct conditions.  
Example: Submitting a signup form with a valid name, email, and password.
🔹 Negative Testing
Providing incorrect, invalid, or unexpected data to check how the system responds.  
Example: Entering `@@@` as a name in the registration form.
🔹 Exploratory Testing
Freely navigating and interacting with the application without a fixed script to discover unexpected defects.  
Example: Trying to skip steps in a multi-step form or back-navigating after submission.
🔹 Boundary Value Testing
Testing at the exact edge of allowed input ranges.  
Example: Entering a 1-character password or a 256-character name.
🔹 Validation Testing
Checking whether the system enforces correct input formats.  
Example: Verifying that email fields reject values without `@` or domain.
🔹 Security-Oriented Testing
Testing authentication and session flows for vulnerabilities.  
Example: Submitting an incorrect OTP to test whether the system correctly rejects it.
---

🧩 Modules Tested
#	Module	Description
1	Signup / Registration	New user account creation form
2	Login System	User authentication with credentials
3	Edit Profile	Updating personal profile information
4	Shipping Address	Address input form for delivery details
5	Checkout / Order Confirmation	Final order placement and payment details
6	Contact / Feedback Form	User communication and feedback submission
7	Multi-Step Form Wizard	Sequential, multi-page data entry flow
8	Two-Factor Authentication (2FA)	OTP-based secondary security verification
---

🖥️ Test Environment
Parameter	Details
Testing Type	Manual (Black-Box)
Browser	Google Chrome (Latest)
OS	Windows
Tools Used	Browser DevTools, Screenshots
Test Design	Test cases based on Valid / Invalid / Edge Case inputs
---


