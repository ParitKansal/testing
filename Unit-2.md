# Unit-2
---

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

### Types of Black Box Testing

- **Equivalence Class Partitioning**: Divides input data into valid and invalid classes to reduce the number of test cases.
  - Valid Class + Invalid Class 1 + Invalid Class 2 + Invalid Class 3 + ...

- **Boundary Value Analysis**: Focuses on testing at the boundaries of input ranges, where errors often occur.

- **Decision Table**: Represents logical relationships between inputs and expected outputs in a table format.

  | **Field**   | **Case 1** | **Case 2** | **Case 3** | **Case 4** |
  |-------------|------------|------------|------------|------------|
  | **Email**   | Valid      | Valid      | Invalid    | Invalid    |
  | **Password**| Valid      | Invalid    | Valid      | Invalid    |
  | **Output**  | Success    | Failure    | Failure    | Failure    |

- **State Transition Testing**: Tests the system's behavior for different states and transitions between those states.  
  ![](https://www.guru99.com/images/2/state_transition.png)

- **Requirement-Based Techniques**: Involves creating test cases based on the specified requirements of the system to ensure they are met.

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


### Model-Based Testing (MBT)

Model-based testing (MBT) is a software testing technique where models (abstract representations) of the system are used to generate test cases. It helps in automating the test case creation process and ensures that all possible scenarios are considered.

#### Key Points:
- **Model Creation**: A model is created to represent the system's behavior, which could include state machines, data flow diagrams, or other forms of abstract representations.
- **Test Case Generation**: From the model, automated tools generate test cases based on predefined criteria, ensuring that the system behaves as expected under various conditions.
- **Types of Models**:
  - **Finite State Machines (FSM)**: Represents the system as a set of states and transitions between those states.
  - **Statecharts**: Extends FSMs by incorporating hierarchical states and actions.
  - **Activity Diagrams**: Used to describe workflows or processes in the system.
  - **Sequence Diagrams**: Shows how objects interact in the system over time.

---
### **Black Box Testing vs. White Box Testing**

| **Aspect**                 | **Black Box Testing**                          | **White Box Testing**                       |
|----------------------------|------------------------------------------------|---------------------------------------------|
| **Definition**             | Tests functionality without code knowledge.    | Tests internal code and structure.          |
| **Focus**                  | System behavior and output.                    | Internal logic and code structure.          |
| **Testers' Knowledge**     | No code knowledge required.                    | Requires knowledge of the code.             |
| **Types of Testing**       | Functional, system, integration, etc.          | Unit testing, code coverage, etc.           |
| **Techniques**             | Equivalence Partitioning, BVA, etc.            | Statement Coverage, Path Coverage, etc.     |
| **Advantages**             | Simple, does not require code knowledge.       | Thorough, identifies internal defects.      |
| **Typically Done By**      | Software testers                               | Software developers                         |

---
