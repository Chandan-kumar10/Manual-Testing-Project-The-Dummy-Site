
#  Test Case Document – The Dummy Site

##  Project Details

* **Project Name:** Manual Testing – The Dummy Site
* **Tester:** Chandan Kumar
* **Testing Type:** Manual Testing
* **Environment:** Web (Chrome Browser)

---

#  MODULE 1: SIGNUP

---

##  Test Case 1: Successful Signup with Valid Email

###  Module

Signup

### 🧾 Description

Verify that the system allows user registration with valid email format.

###  Preconditions

User is on Signup page.

###  Steps to Execute

1. Enter valid email: `user@gmail.com`
2. Enter valid password
3. Click on Signup

###  Test Data

Valid email and password

###  Expected Result

User should be registered successfully.

###  Actual Result

User registered successfully.

### 📊 Status

Pass

###  Severity

High

---

##  Test Case 2: Signup with Invalid Email Format

###  Module

Signup

### 🧾 Description

Verify that the system rejects invalid email formats.

###  Preconditions

User is on Signup page.

###  Steps to Execute

1. Enter email: `prince!12@q.q`
2. Fill remaining fields
3. Click on Signup

### 📥 Test Data

Invalid email

###  Expected Result

System should display validation error.

###  Actual Result

System accepts invalid email and allows signup.

### 📊 Status

Fail

###  Severity

High

---

---

#  MODULE 2: LOGIN

---

##  Test Case 3: Login with Valid Credentials

###  Module

Login

### 🧾 Description

Verify successful login with correct credentials.

###  Steps

1. Enter valid username and password
2. Click Login

###  Expected Result

User should login successfully.

###  Actual Result

Login successful.

### 📊 Status

Pass

---

## Test Case 4: Account Lock After Multiple Failed Attempts

###  Module

Login

### 🧾 Description

Verify that system blocks user after multiple failed login attempts.

###  Steps

1. Enter incorrect password multiple times
2. Observe system response

###  Expected Result

User should be temporarily blocked.

###  Actual Result

User is blocked for 15 minutes.

### 📊 Status

Pass

---

---

#  MODULE 3: PROFILE

---

##  Test Case 5: Name Field Validation

###  Module

Profile

### 🧾 Description

Verify that name field accepts only valid characters.

###  Steps

1. Enter name: `@@kumar`
2. Click Save

###  Expected Result

System should reject special characters.

###  Actual Result

System accepts input and updates profile.

### 📊 Status

Fail

###  Severity

Medium

---

---

#  MODULE 4: SHIPPING

---

##  Test Case 6: Shipping Form with Invalid Data

###  Module

Shipping

### 🧾 Description

Verify that shipping form validates user input.

###  Steps

1. Enter:

   * City: `@@`
   * Postal Code: `@@`
   * Street: `@@@`
2. Submit form

###  Expected Result

System should reject invalid data.

###  Actual Result

Form accepts data and saves address.

### 📊 Status

Fail

###  Severity

High

---

---

#  MODULE 5: CHECKOUT

---

##  Test Case 7: Checkout with Invalid Details

###  Module

Checkout

### 🧾 Description

Verify that checkout process validates user input before confirming order.

###  Steps

1. Enter:

   * Name: `@@@`
   * Zipcode: `!@#`
   * Street: `@@@`
2. Click Place Order

###  Expected Result

System should not confirm order.

###  Actual Result

Order is confirmed successfully.

### 📊 Status

Fail

###  Severity

Critical

---

---

#  MODULE 6: FEEDBACK

---

##  Test Case 8: Feedback Form Validation

###  Module

Feedback

### 🧾 Description

Verify that feedback form validates email and subject.

###  Steps

1. Enter:

   * Email: `prince!12@q.q`
   * Subject: `@321!!11`
2. Submit

###  Expected Result

System should show validation error.

###  Actual Result

Form accepts invalid data.

### 📊 Status

Fail

###  Severity

Medium

---

---

#  MODULE 7: MULTI-STEP FORM

---

##  Test Case 9: Multi-Step Form Validation

###  Module

Multi-Step Form

### 🧾 Description

Verify that each step validates input before proceeding.

###  Steps

1. Enter invalid data in all steps
2. Continue

###  Expected Result

System should validate each step.

###  Actual Result

Form completes successfully.

### 📊 Status

Fail

###  Severity

High

---

---

#  MODULE 8: 2FA

---

##  Test Case 10: OTP Validation

###  Module

2FA

### 🧾 Description

Verify that system rejects incorrect OTP.

###  Steps

1. Enter wrong OTP
2. Submit

###  Expected Result

Verification should fail.

###  Actual Result

OTP accepted and verified.

### 📊 Status

Fail

###  Severity

Critical

---

---
