# Unit-5

### Test Plan Document for Software Testing

A comprehensive test plan serves as a roadmap for the entire testing process, ensuring that all test activities are systematically carried out in alignment with business goals. 

#### **Key components of an effective test plan**
1. **Scope**: Defines what will be tested in the system, ensuring clear objectives are set for the testing phase.
2. **Out of Scope**: Lists the functionalities or areas that will not be tested in this testing cycle.
3. **Timeline**
4. **Resource Allocation / Roles and Responsibilities**
5. **Tools**: Identifies the testing tools and technologies used throughout the testing process.
6. **Environment**: Specifies the test environment configuration, including hardware, software, and network setup.
7. **Deliverables**: Describes the outputs that are expected after each testing phase.
8. **Exit Criteria**: Defines the conditions that must be met before ending a testing phase or project.
9. **Defect Management**: Describes how defects found during testing will be managed, tracked, and resolved.

**Six steps to creating a test plan**
1. **Define the Release Scope**: Identify the features to be tested and clarify out-of-scope elements.  
2. **Schedule Timelines**: Set testing milestones, deadlines, and communicate the schedule.  
3. **Define Test Objectives**: Align testing goals with functional, non-functional requirements, and business needs.  
4. **Determine Test Deliverables**: List and format required documents, specifying audience and purpose.  
5. **Design the Test Strategy**: Define testing levels, types, manual vs. automated testing, and risk management.  
6. **Plan Test Environment and Data**: Specify environment requirements and plan for test data creation and management.

---

**Test Management:**
Test Management involves overseeing the entire software testing process to ensure high-quality testing and delivery. It focuses on organizing, tracking, and controlling testing activities to ensure everything runs smoothly and meets quality standards.

**Test Management Process:**
The process covers the full software testing lifecycle, from planning to execution, with activities like designing test cases, planning, and tracking progress. It ensures that testing is done properly and consistently throughout the project.

**Responsibilities:**
- Collaborate with test analysts to customize templates and establish standards.
- Track and control the testing process during the project.
- Provide clarity on the testing activities for upcoming projects.

**Key Components of Test Management:**

1. **Planning:**
   - **Risk Analysis**: Identifying potential issues in testing.
   - **Test Estimation**: Estimating the time and resources needed.
   - **Test Planning**: Creating a clear plan for how the testing will be conducted.

2. **Execution:**
   - **Testing Activity**: Carrying out the tests.
   - **Issue Management**: Handling any issues or bugs that arise.
   - **Test Reporting and Evaluation**: Documenting the test results and evaluating their success.

**Activities in the Test Process:**
1. **Test Plan**: Outlines the overall testing approach.
2. **Test Design**: Details the specific tests and how they will be implemented.
3. **Test Execution**: Running tests and comparing actual results to expected ones.
4. **Exit Criteria**: Signals when to stop the testing process.
5. **Test Reporting**: Summarizes the test process and results for the current cycle.

---

### Automation Testing

**Automation Testing Types:**
- **Unit Testing**: Tests the smallest piece of code (unit) in isolation during development.
- **Integration Testing**: Combines and tests individual software components to check compatibility and functional requirements.
- **Smoke Testing**: Preliminary check to determine if the software is stable before further testing.
- **Performance Testing**: Assesses system stability and responsiveness under specific loads.
- **Regression Testing**: Ensures that changes haven’t negatively affected existing features.
- **Security Testing**: Identifies security vulnerabilities and risks in the software application.
- **Acceptance Testing**: Confirms if the software meets user approval and business requirements.
- **API Testing**: Validates the functionality, security, and reliability of the API.
- **UI Testing**: Ensures that all elements on the user interface function correctly.

**Test Automation Frameworks:**
- **Linear Framework**: Simple "record and playback" method where test scripts are created and run for each test. Good for beginners or small teams.
- **Modular-Based Framework**: Breaks tests into smaller, independent parts (modules), all controlled by a master script. Requires more planning and is better for experienced testers.
- **Library Architecture Framework**: Builds on the modular framework by organizing tasks into reusable functions. More flexible, but takes longer to set up, so it’s best for testers with more experience.

**Which Tests to Automate:**
- **Monotonous Tests**: Tests that are repetitive and done often can be automated for future use.
- **Tests with Multiple Data Sets**: Tests that need many different data sets can be automated to save time.
- **Business Critical Tests**: Important tests that affect the business can be automated and run regularly.
- **Determinant Tests**: Tests where it’s easy to know if they pass or fail can be automated.
- **Tedious Tests**: Tests that require doing the same thing repeatedly can be automated to reduce errors and improve efficiency.

**Automation Testing Process (Short Points):**
1. **Test Tool Selection**: Choose a tool based on skills, budget, and needs.
2. **Define Scope**: Ensure framework supports scripts, is low maintenance, and has high ROI.
3. **Planning, Design, Development**: Install frameworks and design test cases (e.g., NUnit, JUnit).
4. **Test Execution**: Run tests using the appropriate tool (e.g., NUnit, JUnit).
5. **Maintenance**: Document test results for future reference.


**Criteria to Select Automation Tool:**
1. **Ease of Use**: Choose tools with a user-friendly interface and minimal learning curve.
2. **Support for Multiple Browsers**: Ensure the tool supports cross-browser testing.
3. **Flexibility**: Select a tool that suits the type of testing needed.
4. **Ease of Analysis**: Choose tools with user-friendly reporting and analysis features.
5. **Cost of Tool**: Consider budget and tool efficiency when choosing between free or paid tools.
6. **Availability of Support**: Check if the tool offers community or customer support and training resources.

**Best Practices for Test Automation:**
1. **Plan Self-Contained Test Cases**: Ensure tests are clear, well-written, and easy to understand.
2. **Plan Test Execution Order**: Arrange tests so one creates the state for the next, ensuring smooth execution.
3. **Use Automatic Scheduling Tools**: Choose tools that can schedule tests automatically.
4. **Set Alarms for Test Failures**: Use tools that alert you to test failures and decide whether to continue or abort.
5. **Reassess Test Plans Regularly**: Update test plans as the application evolves to avoid testing outdated features.

**Advantages of Automation Testing:**
1. **Simplifies Execution**: Runs unattended, with results monitored at the end.
2. **Improves Reliability**: Ensures consistent focus on all areas.
3. **Increases Coverage**: Tests more features and complex applications.
4. **Reduces Human Error**: Minimizes mistakes in testing.
5. **Saves Time and Money**: Efficient long-term cost savings.
6. **Faster Defect Detection**: Identifies issues early for quicker fixes.

**Disadvantages of Automation Testing:**
1. **High Initial Cost**: Requires significant time and money investment for tools and setup.
2. **Not 100% Automatable**: Some test cases need human intervention (e.g., design, usability).
3. **Limited Test Types**: Cannot automate tests for user-friendliness or multimedia elements.
4. **Requires Programming Knowledge**: Test scripts need coding skills.
5. **False Positives/Negatives**: Automation may incorrectly show issues or miss them.

**Popular Automation Tools:**

1. **Selenium**: Used for regression testing, supports multiple languages (Java, Python, Ruby), and integrates with frameworks like JUnit and TestNG.
2. **QTP (Quick Test Professional)**: Automated functional testing tool for web and desktop apps, uses VB scripting, supports regression testing.
3. **Sikuli**: GUI-based tool that automates web elements using screenshots, useful for visual testing.
4. **Appium**: Open-source tool for automating app testing across platforms (iOS, Android, Windows).
5. **JMeter**: Open-source Java tool for load testing and measuring the performance of applications.


---

























---

## **1. OO Testing Overview**

### **Class Testing**
- In conventional software, **unit testing** involves testing the smallest functional unit, typically a function or a procedure.  
- In **OO software**, the smallest testable unit is the **class** or an **object** of the class.  
- Testing focuses on two main aspects:  
  1. **Each Method**: Ensuring all methods work as intended.
  2. **State Behavior**: Validating how the object's internal state influences the behavior of methods.

### **State Considerations**
- The state of an object is determined by its attributes (variables) and can impact the behavior of its methods.
- Example:  
  - A class managing a bank account could have states like "open," "closed," and "overdrawn."
  - Methods like `withdraw` or `deposit` may behave differently depending on the account's state.
  
### **Challenges**
- Determining the state of an object during testing can be complex.
- To address this:
  - Additional methods may need to be introduced to inspect the object’s state (e.g., a method to check if an account is open or closed).

---

## **2. OO Class Testing Example**

### **Bank Account Class**
#### **Possible Methods**:
1. `open_account()`
2. `deposit(amount)`
3. `withdraw(amount)`
4. `close_account()`

#### **Possible States**:
1. **Open with Positive Balance**:
   - Allow deposits.
   - Allow withdrawals, with or without overdraft conditions.
2. **Open with Zero or Negative Balance**:
   - Disallow withdrawals.
   - Allow deposits.
3. **Closed**:
   - Disallow all operations.

#### **Behavior Analysis**:
- For **withdrawals**:
  - If balance is positive, withdrawal is allowed.
  - If balance is zero or negative, withdrawal is denied.
- For **overdrafts**:
  - Overdrafts may be permitted only once, depending on the account rules.

#### **Testing Strategy**:
- Introduce a method like `is_open()` or `get_balance()` for testing purposes to determine:
  - If the account is open or closed.
  - The current account balance.

---

## **3. OO Integration Testing**

### **Challenges**:
- Traditional integration strategies like **top-down** or **bottom-up** are not suitable for OO software due to its lack of a hierarchical structure.

### **Approaches**:
1. **Thread-based Testing**:
   - Focuses on testing sets of classes that interact to handle a specific input or event.
   - Each "thread" of interaction is tested individually.
   - Example: A banking system thread might test how a customer deposits money and the impact on balance and state.

2. **Use-based Testing**:
   - Starts with **independent classes** (classes that do not rely on others).
   - Gradually integrates and tests **dependent classes** (those that rely on independent classes).
   - Example: In a library system:
     - First, test the "Book" class (independent).
     - Then test the "Borrower" class (dependent on "Book").

---

## **4. Validation Testing**

### **Black-Box Testing in OO**:
- Tests functionality without focusing on internal implementation.
- **Use cases** are often utilized to derive test cases, ensuring that all possible user interactions with the system are covered.

### **Example**:
- A use case for a library management system might describe the steps for issuing a book:
  1. Search for a book.
  2. Check availability.
  3. Issue the book.

---

## **5. Test Cases and the Class Hierarchy**

### **Hierarchy Testing Considerations**:
1. **Redefined Methods**:
   - Methods redefined in a subclass (overriding methods) must be tested because they represent new code and behavior.
   
2. **Inherited Methods**:
   - Methods inherited from a parent class must also be tested to ensure they behave as expected in the derived class.
   - A subset of the original test cases can often be reused for this purpose.

---

## **6. Types of Testing Approaches**

### **Random Testing**:
- Randomly generates sequences of operations to test various interactions.
- Important to consider the **behavior life sequence** of the class.
- Example:
  - Randomly test sequences like `open_account → deposit → withdraw → close_account` to observe unexpected behaviors.

### **Partition Testing**:
- Similar to **equivalence class partitioning** in traditional software testing.
- Inputs and outputs of the class are divided into partitions or categories, and test cases are designed to cover each partition.

---

## **7. Types of Partition Testing**

### **State-based Partitioning**:
- Focuses on the **states of the class**.
- Identify:
  1. Which operations **change the state**.
  2. Which operations do **not change the state**.
- Design test cases to:
  - Exercise methods while the object is in various states.
  - Validate transitions between states.
  
#### Example:
- For a bank account:
  - Test `withdraw` and `deposit` in states like "open with positive balance" or "open with zero balance."
  - Ensure `close_account` transitions the state to "closed."

---

### **Attribute-based Partitioning**:
- Focuses on the **attributes of the class**.
- Partition methods based on:
  1. Methods that **use the attribute**.
  2. Methods that **modify the attribute**.
  3. Methods that **do not interact with the attribute**.
  
#### Example:
- For a `Car` class with an attribute `fuel_level`:
  - `drive()` uses and modifies `fuel_level`.
  - `refuel()` modifies `fuel_level`.
  - `get_make()` does not interact with `fuel_level`.

---

### **Category-based Partitioning**:
- Focuses on **categorizing methods** by their functionality:
  1. **Initialization Operations**: Set up the object.
  2. **Computational Operations**: Perform calculations or processing.
  3. **Queries**: Retrieve information from the object.
  4. **Termination Operations**: Clean up or finalize the object.

#### Example:
- For a `Robot` class:
  - Initialization: `initialize()`
  - Computational: `calculate_path()`
  - Query: `get_battery_status()`
  - Termination: `shutdown()`

Design specific test cases for each category to ensure all functionalities are tested.

---

By breaking down OO testing into these structured approaches, you can ensure thorough testing of object-oriented software. Each method, state, attribute, and behavior is analyzed to uncover defects and ensure robustness.

