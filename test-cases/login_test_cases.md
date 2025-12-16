# Login Test Cases (Web)

**Feature:** Authentication  
**Page:** Login  
**Priority:** High

## Assumptions
- User is registered in the system
- Login page is accessible

## Test Cases

### TC-LOGIN-001 — Valid login
**Preconditions:** Existing user account  
**Steps:**
1. Open Login page
2. Enter valid username
3. Enter valid password
4. Click "Log In"
**Expected Result:**
- User is redirected to a dashboard/home page
- User name or "Logged in" state is visible

### TC-LOGIN-002 — Invalid password
**Steps:**
1. Open Login page
2. Enter valid username
3. Enter invalid password
4. Click "Log In"
**Expected Result:**
- Error message is displayed
- User remains on login page
- No session is created

### TC-LOGIN-003 — Invalid username
**Steps:**
1. Open Login page
2. Enter invalid username
3. Enter any password
4. Click "Log In"
**Expected Result:**
- Error message is displayed
- No session is created

### TC-LOGIN-004 — Empty fields validation
**Steps:**
1. Open Login page
2. Leave username empty
3. Leave password empty
4. Click "Log In"
**Expected Result:**
- Validation messages appear (required fields)
- Login is not performed

### TC-LOGIN-005 — Password masked
**Steps:**
1. Open Login page
2. Type password in password field
**Expected Result:**
- Password is masked (•••••)