### Test Cases and Test Suite

- **Test Case**: A test case is a triplet [I, S, O], where:
  - **I**: Input data to the system
  - **S**: System state at the time of input
  - **O**: Expected output from the system

- **Test Suite**: A collection of test cases designed to verify the software's functionality and behavior.
  
---

### Types of White Box Testing

- **Statement Coverage**: Ensures that every statement in the code is executed at least once during testing.
- **Branch Coverage**: Ensures that each possible branch (true/false) in the decision points (if-else statements) is executed at least once.
- **Path Coverage**: Ensures that all possible paths through the code are tested, including all combinations of branches.
- **Condition Coverage**: Ensures that each condition in decision statements evaluates to both true and false at least once.
- **Mutation Testing**: Involves making small changes (mutations) to the code to ensure that the test suite can detect the introduced defects.
- **Data Flow-Based Testing**: Focuses on testing how data is defined, used, and manipulated throughout the system, checking for correct data flow and usage across the program.

---

| **Aspect**              | **Static Testing**                            | **Dynamic Testing**                            |
|-------------------------|-----------------------------------------------|-----------------------------------------------|
| **Definition**           | Testing without executing the code.           | Testing by executing the code.                |
| **Type**                 | Verification                                  | Validation                                    |
| **Techniques**           | Code reviews, walkthroughs, static analysis tools. | Unit testing, integration testing, system testing. |
| **Purpose**              | To verify if the software meets specified requirements and design. | To validate if the software functions as expected in real-world scenarios. |
| **Advantage**            | Identifies coding errors, design flaws, and ensures standards compliance. | Detects runtime errors, functional defects, and performance issues. |

### **Static Testing**

- **Review**:
  - **Informal Review**: Casual examination of the software.
  - **Walkthrough**: Step-by-step explanation by the author.
  - **Peer Review**: Review by colleagues for errors.
  - **Inspection**: Formal, structured review with checklists.
- **Static Analysis**:
  - **Data Flow**: Analyzes data movement and usage.
  - **Control Flow**: Examines the flow of control in the code.
  - **Cyclomatic Complexity**: Measures code complexity based on independent paths.

---

  
### Black-Box Test Suite for Palindrome Function
- **Test Case 1:** Normal Palindrome String
- **Test Case 2:** Palindrome with Mixed Case
- **Test Case 3:** Non-Palindrome String
- **Test Case 4:** Empty String
- **Test Case 5:** Single Character String
- **Test Case 6:** String with Special Characters (Palindrome)
- **Test Case 7:** String with Special Characters (Not a Palindrome)
- **Test Case 8:** Maximum Length Palindrome
- **Test Case 9:** Maximum Length Non-Palindrome
- **Test Case 10:** Palindrome with Numbers

### Black-Box Test Suite for Book Search Function
- **Test Case 1:** Book Exists in the Library (Exact Match)
- **Test Case 2:** Book Exists in the Library (Case Insensitive Match)
- **Test Case 3:** Book Does Not Exist in the Library
- **Test Case 4:** Book Exists in the Library with Special Characters in the Name
- **Test Case 5:** Book Exists in the Library with Extra Whitespace
- **Test Case 6:** Book Exists with Partial Name Match
- **Test Case 7:** Empty String Input
- **Test Case 8:** Book Name with Numeric Characters
- **Test Case 9:** Book Name with Multiple Words
- **Test Case 10:** Book Exists in the Library (Matching After File Update)

---
