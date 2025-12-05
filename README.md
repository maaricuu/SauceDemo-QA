🧪 SauceDemo Manual QA Project

## 📋 Project Overview
This repository contains manual QA documentation and evidence for the SauceDemo demo e‑commerce application.  
The goal is to validate core functionalities (login, product listing, cart, checkout, sorting, UI consistency) and identify defects.

---

🎯 Test Plan
- **Objective** Verify functionality, stability, and user interface of SauceDemo demo site.
  
- **Scope** Login/Logout, product listing & details, cart operations, checkout process, sorting & filtering, UI testing.
  
- **Bug Reports**
  - BUG-001: Reset App State does not reset sorting option (Minor/Low)
  - BUG-002: Sidebar remains open after navigation (Minor/Low)
  - BUG-003: Checkout allows numeric input in Name fields (Minor/Low)
  - BUG-004: Locked-out user can bypass login and add to cart (Major/High)
  - BUG-005: ZIP field accepts special characters (Minor/Low)
  - BUG-006: Product image over-zooms on mobile resolution (Minor/Low)
  - BUG-007:*Back navigation on Product Details returns to top of page (Minor/Low)  
    
- **Test Cases**
  
  LOGIN TESTS
  - TC-001: Login with valid credentials (PASS)
  - TC-002: Login with invalid credentials (PASS)
  - TC-003: Login with locked user (PASS)
  - TC-013: Logout functionality (PASS)

  PRODUCT TESTS
  - TC-004: Verify product list loads (PASS)
  - TC-014: Open product details page (PASS)

  CART TESTS
  - TC-005: Add single product to cart (PASS)
  - TC-006: Add multiple products to cart (PASS)
  - TC-007: Remove product from cart (PASS)
  - TC-012: Cart badge updates correctly (PASS)

  CHECKOUT TESTS
  - TC-008: Checkout – enter customer info (PASS)
  - TC-009: Checkout – finish order (PASS)

  SORTING & UI TESTS
  - TC-010: Sorting products Price low-high (PASS)
  - TC-011: Sorting products Name Z-A (PASS)
  - TC-015: UI/Visual consistency check (PASS)
    
- **Environment**  
  - Browsers: Chrome, Firefox, Edge  
  - OS: Windows 10, Windows 11, macOS, Android 14  
  - Test users: `standard_user`, `locked_out_user`, `problem_user`, `performance_glitch_user`
    
- **Risks & Assumptions**  
  - Possible downtime due to maintenance  
  - Demo site changes may affect tests  
  - Limited test users and product catalog

- **Test Types** 
  - Functional Testing
  - Smoke Testing
  - Regression Testing
  - UI Testing

---

🧪 Test Execution Summary
| Metric                     | Value                     |
|----------------------------|---------------------------|
| Total Test Cases Executed  | 15                        |
| Passed                     | 15                        |
| Failed                     | 0                         |
| Bugs Logged                | 7                         |
| Execution Date             | 01–02/12/2025             |
| Browsers Used              | Chrome (Desktop & Mobile) |
| OS                         | Windows 11, Android 14    |

---

🐞 Bug Report
- **Total Bugs:** 7  
- **Severity Breakdown:**  
  - Major: 1 (Locked‑out user bypasses login and adds products to cart)  
  - Minor: 6 (UI, input validation, mobile zoom, navigation issues)  
- **Status:** All bugs logged as *New* on 02/12/2025  

---

🔗 Traceability Matrix
| Requirement / Feature              | Test Case ID | Bug ID   | Notes                                |
|-----------------------------------|--------------|----------|--------------------------------------|
| Login valid/invalid/locked users  | TC-001–003   | BUG-004  | Valid login works, locked user issue |
| Product listing & details         | TC-004, TC-014 | BUG-006 | Product info correct, mobile zoom bug|
| Cart operations                   | TC-005–007, TC-012 | – | Add/remove products, badge updates   |
| Checkout                          | TC-008–009   | BUG-003, BUG-005 | Input validation issues              |
| Sorting                           | TC-010–011   | BUG-001  | Reset App State bug                  |
| Logout                            | TC-013       | BUG-002  | Sidebar remains open after logout    |
| UI consistency                    | TC-015       | BUG-007  | Back navigation scroll issue         |

---

📂 Documentation Links
- [Test Plan](TestPlan_SauceDemo.pdf)
- [Test Cases](TestCases_SauceDemo.xlsx)
- [Bug Report](BugReport_SauceDemo.xlsx)
- [Traceability Matrix](Traceability_matrix.xlsx)
- [Mind Map](MindMap.png)
- [Summary Report](SummaryReport_SauceDemo.docx)
- [Screenshots Folder](Attachments_BugReport/)
 
---

✅ Application Status
- All 15 test cases passed successfully  
- 7 bugs identified (1 major, 6 minor)  
- Core workflows stable and functional  
- Major bug (login bypass) requires fix before production release  
- Application is suitable for demo purposes with noted limitations
