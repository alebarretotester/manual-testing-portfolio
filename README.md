# 🧪 Manual Testing Project: LinkedIn Login Page

This project demonstrates my practical skills in Manual QA, focusing on test scenario design, execution, and bug documentation.

## 📋 Test Cases (Casos de Teste)

### 🔑 Scenario 1: Successful Login with Valid Credentials
*   **Pre-conditions:** User must have a registered account.
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address in the "Email" field.
    3. Enter the correct password in the "Password" field.
    4. Click the "Sign in" button.
*   **Expected Result:** The user is successfully redirected to their LinkedIn Feed home page.
*   **Status:** ✅ PASSED

### ❌ Scenario 2: Login Failure with Incorrect Password
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Enter a valid email address.
    3. Enter an incorrect password.
    4. Click the "Sign in" button.
*   **Expected Result:** An error message appears stating "Wrong password" or "Invalid credentials", and the user remains on the login page.
*   **Status:** ✅ PASSED

### ⚠️ Scenario 3: Login Failure with Empty Fields
*   **Steps:**
    1. Navigate to the LinkedIn login page.
    2. Leave both "Email" and "Password" fields blank.
    3. Click the "Sign in" button.
*   **Expected Result:** Inline validation errors appear alerting the user that the fields are required.
*   **Status:** ❌ FAILED (Example Bug)
