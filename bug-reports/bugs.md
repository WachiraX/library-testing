D:\library-testing\src\__tests__\Auth.test.js
   8:1  error  'describe' is not defined  no-undef
   9:3  error  'describe' is not defined  no-undef
  10:5  error  'test' is not defined      no-undef
  16:7  error  'expect' is not defined    no-undef
  17:7  error  'expect' is not defined    no-undef
  18:7  error  'expect' is not defined    no-undef
  19:7  error  'expect' is not defined    no-undef
  20:7  error  'expect' is not defined    no-undef
  23:5  error  'test' is not defined      no-undef
  29:7  error  'expect' is not defined    no-undef
  30:7  error  'expect' is not defined    no-undef
  33:5  error  'test' is not defined      no-undef
  39:7  error  'expect' is not defined    no-undef
  40:7  error  'expect' is not defined    no-undef
  43:5  error  'test' is not defined      no-undef
  49:7  error  'expect' is not defined    no-undef
  53:3  error  'describe' is not defined  no-undef
  54:5  error  'test' is not defined      no-undef
  68:7  error  'expect' is not defined    no-undef
  69:7  error  'expect' is not defined    no-undef
  73:3  error  'describe' is not defined  no-undef
  74:5  error  'test' is not defined      no-undef
  88:7  error  'expect' is not defined    no-undef
  89:7  error  'expect' is not defined    no-undef
  90:7  error  'expect' is not defined    no-undef
  91:7  error  'expect' is not defined    no-undef
  94:5  error  'test' is not defined      no-undef
  97:7  error  'expect' is not defined    no-undef

D:\library-testing\src\__tests__\Books.test.js
   13:1  error  'describe' is not defined   no-undef
   17:3  error  'beforeAll' is not defined  no-undef
   28:3  error  'describe' is not defined   no-undef
   29:5  error  'test' is not defined       no-undef
   34:7  error  'expect' is not defined     no-undef
   35:7  error  'expect' is not defined     no-undef
   36:7  error  'expect' is not defined     no-undef
   39:5  error  'test' is not defined       no-undef
   44:7  error  'expect' is not defined     no-undef
   46:7  error  'expect' is not defined     no-undef
   47:7  error  'expect' is not defined     no-undef
   48:7  error  'expect' is not defined     no-undef
   49:7  error  'expect' is not defined     no-undef
   53:3  error  'describe' is not defined   no-undef
   54:5  error  'test' is not defined       no-undef
   60:7  error  'expect' is not defined     no-undef
   61:7  error  'expect' is not defined     no-undef
   64:5  error  'test' is not defined       no-undef
   70:7  error  'expect' is not defined     no-undef
   71:7  error  'expect' is not defined     no-undef
   75:3  error  'describe' is not defined   no-undef
   76:5  error  'test' is not defined       no-undef
   81:7  error  'expect' is not defined     no-undef
   82:7  error  'expect' is not defined     no-undef
   83:7  error  'expect' is not defined     no-undef
   84:7  error  'expect' is not defined     no-undef
   87:5  error  'test' is not defined       no-undef
   92:7  error  'expect' is not defined     no-undef
   93:7  error  'expect' is not defined     no-undef
   97:3  error  'describe' is not defined   no-undef
   98:5  error  'test' is not defined       no-undef
  112:7  error  'expect' is not defined     no-undef
  114:9  error  'expect' is not defined     no-undef
  118:5  error  'test' is not defined       no-undef
  127:7  error  'expect' is not defined     no-undef
  128:7  error  'expect' is not defined     no-undef
  132:3  error  'describe' is not defined   no-undef
  133:5  error  'test' is not defined       no-undef
  136:7  error  'expect' is not defined     no-undef

D:\library-testing\src\app.js
    6:29  error  'db' is assigned a value but never used  no-unused-vars
  114:25  error  'next' is defined but never used         no-unused-vars

D:\library-testing\src\controllers\BorrowingController.js
  193:15  error  'db' is assigned a value but never used  no-unused-vars

D:\library-testing\src\controllers\DashboardController.js
  2:9  error  'db' is assigned a value but never used  no-unused-vars 

D:\library-testing\src\routes\borrowing.js
  5:22  error  'requireAdmin' is assigned a value but never used  no-unused-vars

✖ 72 problems (72 errors, 0 warnings)

# Bug Reports - Phase 1: Static Analysis

| Bug ID | Title (หัวข้อ) | File Location (ไฟล์ที่พบ) | Severity | Issue Link |
| :---    | :---  | :--- | :--- | :--- |
| BUG-001 | Security: `requireAdmin` middleware is imported but never used | src/routes/borrowing.js | High | #2 |
| BUG-002 | Code Quality: `db` connection is imported but not used | src/app.js | Low | #3 |
| BUG-003 | Code Quality: `next` function is defined but never used | src/app.js | Low | #4 |
| BUG-004 | Code Quality: Unused `db` variable in BorrowingController | src/controllers/BorrowingController.js | Low | #5 |
| BUG-005 | Code Quality: Unused `db` variable in DashboardController | src/controllers/DashboardController.js | Low | #6 |