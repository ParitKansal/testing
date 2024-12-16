# Unit - 3

### Different integration strategies

| **Integration Strategy**               | **Description**                                                                                                                                                  | **Advantages**                                                                                                               | **Disadvantages**                                                                                                        | **Best For**                                                     |
|----------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------|
| **Big Bang Integration (Nonincremental)** | All components are combined and tested as a whole after each unit has been tested individually.                                                                  | - Quick as it requires fewer initial setups<br> - No need for stubs or drivers                                               | - Difficult to isolate issues<br> - Errors are harder to trace<br> - Risky for large projects                             | Small, simple systems                                           |
| **Bottom-Up Integration**              | Testing begins with the lowest-level modules and progresses upward. Uses **test drivers** to simulate higher-level modules.                                       | - Good for performance-focused systems<br> - Easier to create drivers for lower-level modules<br> - Efficient for OOP        | - UI or main modules tested last<br> - May delay functionality testing                                                    | Object-oriented, real-time, performance-critical systems         |
| **Top-Down Integration**               | Testing starts with the top-level modules and progresses downward, using **stubs** to simulate lower-level modules.                                              | - Allows testing of main functionality early<br> - Detects design errors at higher levels sooner                             | - Stubs for lower-level modules can be complex<br> - Many stubs may be needed, increasing test setup time                 | Systems where top-level functionality needs early validation    |
| **Sandwich Testing**                   | Combines top-down and bottom-up approaches by focusing on a **target middle layer**. Simultaneous testing on top and bottom layers converges at the middle layer. | - Top and bottom layers can be tested in parallel<br> - Reduces need for excessive stubs and drivers                         | - Middle layer must be carefully chosen<br> - Less thorough testing of individual modules before integration              | Multi-layered systems requiring simultaneous top-down & bottom-up testing |
| **Modified Sandwich Testing Strategy** | Tests top, middle, and bottom layers in parallel, with targeted use of stubs and drivers. Middle layer tested independently, minimizing stubs and drivers.       | - Efficient parallel testing across layers<br> - Reduces stubs and drivers<br> - Facilitates focused testing on middle layer | - Complex setup as it combines both stubs and drivers<br> - Requires careful layer separation to avoid conflicts          | Systems with three clear layers and independent layer interactions |

----

### System Testing

System testing is a comprehensive testing phase where the entire system is tested as a whole to ensure it meets specified requirements and functions correctly.

#### Types of System Testing

1. **Functional Testing**
2. **Structure Testing**
3. **Performance Testing**
4. **Acceptance Testing**
5. **Installation Testing**

---

### Impact of Requirements on System Testing

- **Clear Requirements Make Testing Easier**: When requirements are clearly stated, it’s easier to create tests that check whether the software meets those requirements.
- **Good Use Cases Simplify Functional Testing**: If the requirements are written as clear, detailed use cases (descriptions of how users will interact with the system), functional testing becomes easier because testers know exactly what to look for.
- **Clear Subsystem Design Aids Structure Testing**: If the system is broken down well into modules or subsystems, it’s easier to test the internal structure. A well-organized structure means structure testing can focus on individual components without confusion.
- **Nonfunctional Requirements Guide Performance Testing**: Requirements for things like speed, scalability, and reliability help testers set up accurate performance tests. Without these, it’s hard to know what to test or what results to expect.

---

### **Structure Testing**

Structure testing is a type of testing where the internal workings or structure of the system are tested directly. This is also known as **white-box testing** because testers need knowledge of the code and system internals to carry out these tests effectively.

#### Goal of Structure Testing
The primary aim of structure testing is to **ensure that all possible paths within the system’s design are tested**. This means thoroughly covering how each part of the system interacts with others and behaves with various inputs and outputs.

#### Key Aspects of Structure Testing

1. **Testing Input and Output Parameters**:
   - Each component or module in the system will have inputs and outputs.
   - Structure testing ensures that all possible inputs are tested, and all expected outputs are verified, so there’s no unexpected behavior or missed scenarios.

2. **Component and Call Coverage**:
   - Every component (or module) within the system should be tested at least once.
   - Every component should also be tested with all possible "callers"—components or functions that interact with it.
   - This ensures that all parts of the system can work together and communicate as expected.

3. **Conditional and Iteration Testing**:
   - Just as in **unit testing** (testing individual components), structure testing includes checking **conditional statements** (like `if` statements) and **loops**.
   - Conditional testing checks if the code correctly handles different logical paths.
   - Iteration testing ensures loops in the code execute correctly and handle different numbers of repetitions without errors.

---

### **Functional Testing**

Functional testing is a type of testing focused on verifying that the system's functionality aligns with the requirements. This type of testing is also called **black box testing** because testers do not need to know the internal workings or code structure of the system. Instead, they only focus on what the system should do, based on user requirements.

#### Goal of Functional Testing
The main objective is to **ensure the system's functionality works as intended**. Testers check whether the system’s features, inputs, and outputs behave as described in the requirements.

#### Key Aspects of Functional Testing

1. **Requirement-Based Test Cases**:
   - Test cases for functional testing are created based on the requirements analysis document or, ideally, the **user manual**.
   - These test cases are designed to cover all key functions, or **use cases**, ensuring that the system meets all user needs.
   - The idea is to check if each function performs as expected and handles all specified inputs and outputs correctly.

2. **System as a Black Box**:
   - In functional testing, the system is treated as a **black box**—testers only see the inputs they provide and the outputs they receive.
   - They do not look into the code or internal logic; they only care about whether the system’s observable behavior matches the requirements.

3. **Reusing Unit Test Cases and Creating New Ones**:
   - Some **unit test cases** (which test individual components) may be reused if they cover similar functions.
   - However, new test cases are often developed with an **end-user perspective** to ensure the software meets user expectations and handles real-world usage scenarios.

---

### **Performance Testing**

Performance testing is a type of testing that focuses on evaluating how well the system performs under various conditions. This testing goes beyond functionality to assess the system's stability, speed, scalability, and response to different loads or environments. Here’s an organized breakdown of different types of performance testing:

#### 1. Stress Testing
   - **Purpose**: To test the limits of the system under extreme conditions.
   - **Checks**: Maximum number of users, peak demands, and extended operation time.

#### 2. Volume Testing
   - **Purpose**: To evaluate the system's ability to handle large amounts of data.
   - **Checks**: System behavior and performance when processing large datasets.

#### 3. Configuration Testing
   - **Purpose**: To ensure the system works across different software and hardware setups.
   - **Checks**: Compatibility with various configurations of operating systems, devices, and networks.

#### 4. Compatibility Testing
   - **Purpose**: To test if the system works with older versions of itself or with existing systems.
   - **Checks**: Backward compatibility with older versions and integration with related systems.

#### 5. Security Testing
   - **Purpose**: To ensure the system’s security features are effective.
   - **Checks**: Attempts to breach or bypass security controls to validate protection levels.

#### 6. Timing Testing
   - **Purpose**: To evaluate how quickly the system responds to inputs and completes tasks.
   - **Checks**: Response times, latency, and time taken to perform critical functions.

#### 7. Environmental Testing
   - **Purpose**: To test how well the system withstands different environmental conditions.
   - **Checks**: System tolerances for heat, humidity, movement, and portability.

#### 8. Quality Testing
   - **Purpose**: To ensure the system is reliable, easy to maintain, and available as expected.
   - **Checks**: Reliability, maintainability, and availability under normal and adverse conditions.

#### 9. Recovery Testing
   - **Purpose**: To verify the system’s ability to recover from errors or data loss.
   - **Checks**: System response and recovery mechanisms for error handling and data recovery.

#### 10. Human Factors Testing
   - **Purpose**: To evaluate the usability of the system’s interface.
   - **Checks**: User experience, ease of navigation, and interaction with the user interface.



---

### **Acceptance Testing**

Acceptance testing is the final phase in the software testing process, ensuring that the system is ready for deployment and use by the client or end-users. The goal is to **demonstrate that the system is ready for operational use** and meets the specified requirements and expectations.

#### Key Aspects of Acceptance Testing

1. **Goal: System Readiness for Use**:
   - Acceptance testing is conducted to confirm that the system is functional, reliable, and ready for the client or sponsor to use in their real-world environment.

2. **Client/Sponsor Involvement**:
   - Unlike other types of testing, where the developers and testers conduct the tests, **the client or sponsor** chooses the specific tests and performs the acceptance testing.
   - The focus is on ensuring the system meets business needs, rather than technical correctness.

3. **Integration Tests Reused**:
   - Some tests that were conducted earlier during **integration testing** (when different components of the system were combined and tested together) can be reused in acceptance testing.

4. **Client-Performed Testing**:
   - Acceptance testing is performed **by the client**, not the developer or tester. This helps ensure that the software works from the user's perspective and fulfills their requirements.

---

### Additional Testing Phases in Acceptance Testing

1. **Alpha Testing**:
   - **Alpha testing** is done at the developer's site and is typically performed by the sponsor or a select group of users.
   - The software is used in a controlled setting, where developers are available to fix any bugs immediately if they are discovered during the testing phase.
   - It’s essentially the last round of internal testing before the software is released to a broader group.

2. **Beta Testing**:
   - **Beta testing** takes place at the sponsor's site, not in the developer’s controlled environment.
   - The software is tested in a **realistic environment**, where it gets a more natural "workout" from actual users.
   - Since the developer is not directly present, this testing gives a clearer picture of how the software will behave when it’s released to the public.
   - However, it can lead to a situation where potential customers or users might get discouraged if they encounter bugs or issues, affecting the software’s reputation.

### Why Acceptance Testing Is Crucial
- **Majority of bugs are found by the client** after the software is in use. Developers and testers typically catch most of the technical bugs, but users often encounter new, practical issues once they start using the system in real-world conditions.
- This is why acceptance testing is vital—it ensures the system works from the user’s point of view before it is fully released.

---

| **Aspect**                | **Functional Testing**                                 | **Non-Functional Testing**                            |
|---------------------------|---------------------------------------------------------|-------------------------------------------------------|
| **Definition**             | Tests the functionality of the system based on specified requirements. | Tests non-functional aspects like performance, usability, and reliability. |
| **Focus**                  | Focuses on what the system does (i.e., features, behaviors). | Focuses on how well the system performs or behaves under certain conditions. |
| **Example**                | Verifying login functionality, payment processing, or data retrieval. | Testing system performance, scalability, security, or user experience. |
| **Test Basis**             | Requirements or use cases describing system features. | System's behavior under stress, performance benchmarks, and constraints. |
| **Type of Tests**          | Black-box testing, functional tests, integration tests. | Performance testing, load testing, stress testing, usability testing, security testing. |
| **Test Results**           | The system either performs the required functions correctly or fails to do so. | Results focus on metrics like speed, stability, and user satisfaction. |
| **Test Example**           | Does the login page allow a user to log in with correct credentials? | How fast does the website load under heavy traffic? |
| **Test Tools**             | Functional testing tools like Selenium, JUnit, etc. | Performance testing tools like LoadRunner, JMeter, etc. |
| **End Goal**               | To ensure all features and functions of the system work as expected. | To evaluate the system's behavior under different conditions and its performance standards. |

---
---

## **Defect Bash**

- **Group Activity**: Multiple testers or developers collaborate to identify defects.
- **Time-Constrained**: Typically lasts a few hours (e.g., 2-4 hours).
- **Exploratory Testing**: Focuses on free-form testing, not following predefined test cases.
- **Wide Coverage**: Aims to explore many parts of the application quickly.
- **No Formal Test Plan**: Informal, based on testers' instincts and experience.
- **Focus on Defects**: Main goal is to discover as many defects as possible.
- **Collaborative**: Encourages teamwork and knowledge sharing.
- **Fun & Competitive**: May include gamification or rewards for finding defects.
  
### **Benefits**:
- Increased defect discovery.
- Enhanced team collaboration.
- Focus on critical issues before release.
- Boosts team morale.

### **Use Cases**:
- Before software release.
- After major changes or updates.
- At the end of a testing cycle.

### **Limitations**:
- Superficial coverage of certain areas.
- Defects found may not always be critical.


----
### **Scalability Testing**

Scalability testing evaluates how well a system can handle increasing loads, traffic, or data volume. The goal is to ensure that the system can maintain performance as demands grow and to identify any bottlenecks that could affect its ability to scale.

### **Key Aspects**:
1. **Vertical Scalability (Scaling Up)**: Increasing capacity on a single server (e.g., more CPU, RAM).
2. **Horizontal Scalability (Scaling Out)**: Adding more servers or resources to distribute load.

### **Types of Scalability Testing**:
- **Load Testing**: Assess performance under expected loads.
- **Stress Testing**: Test the system beyond its limits to find failure points.
- **Volume Testing**: Check how the system handles large amounts of data.
- **Concurrency Testing**: Evaluate performance with multiple simultaneous users.
- **Endurance Testing**: Test performance over extended periods.

### **Process**:
1. Define expected load and performance metrics (response time, resource usage).
2. Simulate load using tools (e.g., JMeter, LoadRunner).
3. Monitor performance (e.g., CPU, memory).
4. Identify bottlenecks and failure points.
5. Optimize based on test results (e.g., improve caching, load balancing).

### **Benefits**: 
- Ensures the system performs well under increasing demand.
- Identifies weaknesses to improve before scaling up in production.

---

### **Reliability Testing**

Reliability testing ensures that a software application or system performs consistently and correctly under expected conditions for a specified period of time. The goal is to verify that the system can operate without failure over time, handling errors gracefully and providing a stable user experience.

### **Key Objectives**:
1. **Consistency**: Ensure the system behaves as expected without crashes or errors under normal usage conditions.
2. **Fault Tolerance**: Verify how well the system handles failures (e.g., crashes, unexpected shutdowns).
3. **Error Handling**: Ensure the system can recover from errors without affecting overall functionality.
4. **Uptime**: Ensure the system maintains continuous operation without interruption for extended periods.

### **Types of Reliability Testing**:
1. **Stability Testing**: Verify the system operates without crashing or freezing over time.
2. **Failure Testing**: Simulate faults (e.g., network loss, power failure) to check if the system can recover gracefully.
3. **Recovery Testing**: Test how well the system can recover from failures and resume normal operations.
4. **Mean Time Between Failures (MTBF)**: Measure the average time the system operates without failure.
5. **Endurance Testing**: Test the system's behavior under a prolonged load or continuous operation.

### **Process**:
1. **Simulate Real-World Conditions**: Test the system under typical usage patterns to ensure stability.
2. **Introduce Failures**: Simulate faults or unexpected conditions (e.g., server crashes, network failures) to check the system’s reliability.
3. **Monitor Performance**: Track system performance over time, including response times, uptime, and error rates.
4. **Analyze Results**: Identify weaknesses in error handling, recovery, and uptime.

### **Tools**:
- **LoadRunner**
- **Apache JMeter**
- **Chaos Monkey** (for simulating failures)
- **Selenium** (for automation in failure scenarios)

### **Benefits**:
- Ensures high availability and stability of the system.
- Reduces the risk of system downtime and improves user trust.
- Helps identify and address reliability issues before the system goes live.
