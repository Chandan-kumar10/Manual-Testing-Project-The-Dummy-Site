#  Bug Report – The Dummy Site

##  Project Details

- **Project Name:** Manual Testing – The Dummy Site  
- **Tester:** Chandan Kumar  
- **Testing Type:** Manual Testing  
- **Environment:** Web (Chrome Browser)



 <br> 
 <br> 

## 🔴 Bug 1: Invalid Email Formats Accepted

### 📍 Module
Signup / Feedback

### 🧾 Description
The system accepts invalid email formats without performing proper validation checks.

### 🔁 Steps to Reproduce
1. Open the Signup page  
2. Enter email: `prince!12@q.q`  
3. Fill remaining required fields  
4. Click on Submit  

### ✅ Expected Result
The system should validate the email format and reject invalid email addresses.

### ❌ Actual Result
The system accepts the invalid email and allows successful submission.

### 🎯 Impact
Invalid user data is stored, which can lead to communication failures.

### ⚠️ Severity: High  
### 🚨 Priority: High  





 <br>
<br> 


## 🔴 Bug 2: Name Field Accepts Special Characters

### 📍 Module
Edit Profile

### 🧾 Description
The name field accepts special characters and invalid input values.

### 🔁 Steps to Reproduce
1. Open Profile Edit page  
2. Enter name: `@@kumar`  
3. Click Save  

### ✅ Expected Result
The name field should accept only alphabetic characters.

### ❌ Actual Result
The system accepts special characters and updates the profile.

### 🎯 Impact
Leads to data inconsistency and poor data quality.

### ⚠️ Severity: Medium  
### 🚨 Priority: Medium  







 <br> 
  <br> 


## 🔴 Bug 3: Shipping Form Accepts Invalid Data

### 📍 Module
Shipping Address

### 🧾 Description
The shipping form does not validate input fields such as city, postal code, and street.

### 🔁 Steps to Reproduce
1. Open Shipping form  
2. Enter the following:
   - City: `@@`  
   - Postal Code: `@@`  
   - Street: `@@@`  
3. Submit the form  

### ✅ Expected Result
The system should validate inputs and reject invalid data.

### ❌ Actual Result
The form accepts invalid inputs and saves the address.

### 🎯 Impact
Incorrect address data may be stored, affecting delivery processes.

### ⚠️ Severity: High  
### 🚨 Priority: High  






 <br> 
 <br> 

## 🔴 Bug 4: Checkout Accepts Invalid Order Details

### 📍 Module
Checkout / Payment

### 🧾 Description
The checkout process allows order confirmation even with invalid input data.

### 🔁 Steps to Reproduce
1. Navigate to Checkout page  
2. Enter the following:
   - Name: `@@@`  
   - Zipcode: `!@#$@#!`  
   - Street: `@@@!#`  
3. Click on Place Order  

### ✅ Expected Result
The system should validate input data before confirming the order.

### ❌ Actual Result
The order is successfully confirmed despite invalid data.

### 🎯 Impact
This leads to critical business logic failure and invalid transaction records.

### ⚠️ Severity: Critical  
### 🚨 Priority: High  






 <br> 
 <br> 

## 🔴 Bug 5: Feedback Form Accepts Invalid Input

### 📍 Module
Feedback

### 🧾 Description
The feedback form accepts invalid email formats and meaningless subject inputs.

### 🔁 Steps to Reproduce
1. Open Feedback form  
2. Enter:
   - Email: `prince!12@q.q`  
   - Subject: `@321!!11`  
3. Submit the form  

### ✅ Expected Result
The system should validate email format and subject input.

### ❌ Actual Result
The system accepts invalid data and shows a success message.

### 🎯 Impact
Poor quality data is stored, reducing effectiveness of feedback system.

### ⚠️ Severity: Medium  
### 🚨 Priority: Medium  






 <br> 
 <br> 

## 🔴 Bug 6: Multi-Step Form Missing Validation

### 📍 Module
Multi-Step Wizard

### 🧾 Description
The multi-step form allows users to proceed with invalid inputs without validation at each step.

### 🔁 Steps to Reproduce
1. Open Multi-step form  
2. Enter:
   - Name: `@@@#$`  
   - City: `123,890`  
   - Street: `@@`  
3. Proceed through all steps  

### ✅ Expected Result
Each step should validate user input before allowing progression.

### ❌ Actual Result
The form completes successfully with invalid data.

### 🎯 Impact
Workflow integrity is compromised and invalid data is collected.

### ⚠️ Severity: High  
### 🚨 Priority: High  









 <br> 
 <br> 

## 🔴 Bug 7: 2FA Authentication Bypass

### 📍 Module
Two-Factor Authentication (2FA)

### 🧾 Description
The system incorrectly verifies an invalid OTP, allowing unauthorized access.

### 🔁 Steps to Reproduce
1. Navigate to 2FA verification page  
2. Enter an incorrect OTP  
3. Submit  

### ✅ Expected Result
The system should reject incorrect OTP and deny access.

### ❌ Actual Result
The system accepts the incorrect OTP and grants access.

### 🎯 Impact
This is a critical security vulnerability that can allow unauthorized users to access accounts.

### ⚠️ Severity: Critical  
### 🚨 Priority: High  








 <br> 
 <br> 
 <br> 


## 🟢 Observation: Login Rate Limiting

### 📍 Module
Login

### 🧾 Description
After multiple failed login attempts, the system temporarily blocks the user.

### ✅ Expected Result
User should be blocked for a certain time after repeated failures.

### ✔️ Actual Result
System correctly blocks user for 15 minutes.

### 🎯 Impact
This is a security feature to prevent brute force attacks.
