# 🧪 Manual Testing Portfolio: Test Cases & Bug Documentation

Welcome to my Quality Assurance repository! This portfolio showcases my practical skills as a **Manual QA Engineer**, focusing on test scenario design, test execution, comprehensive documentation, and bug reporting.

With a professional background in **Content Moderation at Accenture**, I apply a sharp eye for detail, critical thinking, and strict adherence to guidelines to ensure software quality and exceptional user experiences.

---

## 📌 Project Overview
This repository contains end-to-end manual testing artifacts for high-traffic web applications, split into three core modules:
1. **LinkedIn Login Page Automation & Manual Scenarios**
2. **Standard Web Authentication Suite (Login & Security)**
3. **E-commerce Shopping Cart & Promotion Engine (Features & Real Bug Reports)**

---

## 🔑 Project 1: LinkedIn Login Page Validation

Demonstration of core test scenarios for user authentication on a professional networking platform.

### Scenario 1: Successful Login with Valid Credentials
*   **Pre-conditions:** User must have an active registered account.
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address in the "Email" field.
    3. Enter the correct password in the "Password" field.
    4. Click the "Sign in" button.
*   **Expected Result:** The user is successfully redirected to their LinkedIn Feed home page.
*   **Status:** ✅ PASSED

### Scenario 2: Login Failure with Incorrect Password
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address.
    3. Enter an incorrect password.
    4. Click the "Sign in" button.
*   **Expected Result:** An error message appears stating "Wrong password" or "Invalid credentials", and the user remains on the login page.
*   **Status:** ✅ PASSED

### Scenario 3: Login Failure with Empty Fields
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Leave both "Email" and "Password" fields blank.
    3. Click the "Sign in" button.
*   **Expected Result:** Inline validation errors appear alerting the user that the fields are required.
*   **Status:** ❌ FAILED *(See Bug Report methodology applied below)*

---

## 🔐 Project 2: Comprehensive Authentication Test Suite

A complete verification matrix mapped out using standard QA test case structuring.

| ID | Test Scenario | Execution Steps | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC-001** | Login with valid credentials | Input correct email and password. Click "Login". | User successfully enters the dashboard area. | **Pass** |
| **TC-002** | Login with incorrect password | Input correct email and wrong password. Click "Login". | Error message: "Incorrect password". Login blocked. | **Pass** |
| **TC-003** | Login with empty fields | Leave email and password blank. Click "Login". | Validation message requesting required fields. | **Pass** |
| **TC-004** | Invalid email format entry | Type "user123" (missing @) and password. Click "Login". | System blocks submission, warning of invalid email format. | **Pass** |
| **TC-005** | Password recovery flow | Click "Forgot password", enter a valid email address. | Reset link email sent successfully to the user's inbox. | **Pass** |

---

## 🛒 Project 3: E-commerce Shopping Cart Suite

Functional validation of an e-commerce checkout flow, tracking state management and edge cases.

| ID | Test Scenario | Execution Steps | Expected Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **TC-006** | Add product to cart | Click on a product and press the "Add to Cart" button. | Item is added; cart badge counter increments from 0 to 1. | **Pass** |
| **TC-007** | Modify item quantity | Access the cart and change item quantity from 1 to 2 units. | Total price doubles and updates dynamically. | **Pass** |
| **TC-008** | Remove product from cart | Click the "Remove" button or the trash icon on the item. | Product disappears; screen displays "Your cart is empty". | **Pass** |
| **TC-009** | Stock limit enforcement | Try adding 99 units of a product that only has 5 in stock. | System blocks action, displaying "Out of stock / Limited limit". | **Pass** |

### 🪲 Associated Bug Report (Defect Documentation)

*   **Bug ID:** BUG-001
*   **Title:** Valid discount coupon "DESC20" does not update the total price in the shopping cart
*   **Severity:** High
*   **Environment:** Google Chrome (v122.0) / macOS Sonoma

#### 📋 Steps to Reproduce:
1. Navigate to the "Manual QA Book" product page.
2. Click the **"Add to Cart"** button.
3. Proceed to the Shopping Cart checkout page.
4. Locate the "Coupon Code" field and type **"DESC20"** (A valid 20% off coupon).
5. Click the **"Apply"** button.

#### 🎯 Results Logged:
*   **Expected Result:** The system should validate the coupon, display "Coupon applied successfully", and subtract 20% from the order's final total price.
*   **Actual Result (The Bug):** The system displays the green message "Coupon applied successfully", but the checkout final price **remains exactly the same (€25.00)**, executing no discount deduction.

---

## 🛠️ Skills & Tooling Demonstrated
*   **QA Methodologies:** Black Box Testing, Boundary Value Analysis, Equivalence Partitioning, Regression Testing.
*   **Documentation:** Test Cases, Defect Lifecycle Tracking, Technical Writing.

---

## 📚 📖 My Learning Journey & Knowledge Base

In this section, I document the theoretical foundations, terminology, and testing mindsets I am actively mastering during my self-taught path.

👉 **[Access my Technical Study Guide](./study-guide.md)**  
*Click the link above to view notes, detailed methodologies, pros/cons of exploratory testing, and real-world testing analogies (such as the Safety Elevator and the Car Mechanic analogies).*
