| **Aspect**              | **Description**                                                                                                                                       |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Error**               | Occurs during the process of writing a program, usually due to a programmer's misunderstanding or mistake.                                           |
| **Fault or Bug or defect**| The manifestation of one or more errors in the program, commonly referred to as a bug or defect.                                                     |
| **Failure**             | Happens when a faulty piece of code is executed, leading to an incorrect state that propagates to the program's output.                             |

![](https://i.ibb.co/g7cMyHN/Untitled.png)

---
                
### Basics of Software Testing

1. **Quality Requirements**:  
   Industrial products are spot-checked to meet planned standards. Flawed products necessitate design or production changes.  

2. **Software is Intangible**:  
   Unlike physical products, software cannot be tested hands-on, making quality assessment challenging.  

3. **Faulty Software Issues**:  
   Unreliable software can cause financial loss, damage reputations, or pose safety risks, as in the case of malfunctioning autopilot systems.  

4. **Importance of Testing**:  
   Software testing ensures quality by identifying issues during development, reducing risks, and preventing failures or crashes. It is critical but complex.  

-------------

### Objectives of Software Testing  

1. **Finding Defects**: Identify bugs or flaws in the software.  
2. **Quality Assurance**: Build confidence in the product and assess its quality.  
3. **Requirement Fulfillment**: Ensure compliance with business needs and user agreements.  
4. **Defect Prevention**: Prevent the occurrence of future issues.  
5. **Customer Confidence**: Enhance user trust and satisfaction.

----

### Principles of Software Testing  

1. **Testing Shows the Presence of Defects**:  
   Testing can reveal defects but cannot guarantee their complete absence. It reduces defects but does not eliminate them entirely.  

2. **Defect Clustering**:  
   A small percentage of modules often contains the majority of defects, aligning with the **Pareto Principle** (80% of defects originate from 20% of modules).  

3. **Exhaustive Testing is Impossible**:  
   Testing all possible inputs and conditions is impractical due to excessive cost and effort.  

4. **Pesticide Paradox**:  
   Repeating the same tests repeatedly will not uncover new bugs. Test cases must be reviewed and updated to find additional issues.  

5. **Absence of Errors Fallacy**:  
   Even if software is mostly bug-free, it is unusable if it does not meet user requirements. Functional alignment is critical.  

6. **Early Testing**:  
   Detecting defects in early stages of the SDLC is less costly and ensures better software performance. Testing should start at the requirement analysis phase.  

7. **Context-Dependent Testing**:  
   The testing approach varies based on the software context. For instance, testing an e-commerce website differs significantly from testing a mobile app.

---

### Key Concepts in Software Testing  

1. **Program Requirements**:  
   Products, including software, are designed based on specific requirements that outline the expected functions. The tester’s understanding of these requirements during testing determines the expected behavior, even if the requirements evolve during development.

2. **Program Correctness**:  
   The goal of testing is not to prove program correctness but to identify defects. Correctness is theoretically established through mathematical proofs based on formal specifications and the program code. Testing, on the other hand, is used to find errors in the program, but completeness in testing does not guarantee an error-free program.

3. **Program Behavior**:  
   Program behavior can be specified in natural language, but this can be ambiguous. A more formal method, such as using a **state transition diagram** (or state diagram), helps specify behavior by defining the program's state and the transitions between states, making it clearer and less open to interpretation.

---

| **Aspect**          | **Testing**                                        | **Debugging**                                         |
|---------------------|----------------------------------------------------|------------------------------------------------------|
| **Definition**       | The process of evaluating software to identify defects. | The process of finding and fixing defects in code.  |
| **Objective**        | To detect errors or bugs in the software.         | To resolve and fix identified issues or bugs.       |
| **Focus**            | Verifying that the software meets requirements and behaves as expected. | Correcting specific defects or failures in the code. |
| **Scope**            | Broad, involving tests across the entire system.  | Narrow, focusing on fixing specific issues.         |
| **Performed By**     | Testers or QA engineers.                          | Developers or programmers.                          |
| **Timing**           | Occurs during the software development lifecycle (typically before debugging). | Happens after defects are found during testing.    |
| **Outcome**          | Detection of errors or failures.                  | Fixing the root cause of the defect.                |
| **Tools Used**       | Testing frameworks, test cases, and automation tools. | Debuggers, code analysis, and logging tools.        |

---


| **Aspect**               | **Metrics**                                  | **Measurement**                              |
|---------------------------|----------------------------------------------|---------------------------------------------|
| **Definition**            | Standards or units used for evaluating attributes of a project or process. | Quantitative indication of a specific attribute of a product or process. |
| **Purpose**               | Evaluate and compare quality or performance using a defined scale. | Provide numerical values for specific attributes. |
| **Scope**                 | Broader; used for analysis and decision-making. | Narrower; raw data that feeds into metrics. |
| **Usage**                 | Helps in assessing and improving processes. | Captures specific values for tracking. |  

----
### **Verification Testing vs. Validation Testing**  

| **Aspect**                  | **Verification Testing**                                                                                     | **Validation Testing**                                                                                 |
|-----------------------------|------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|
| **Definition**               | Ensures all development elements meet specified standards and protocols.                                   | Ensures the final product meets stakeholder and customer requirements.                               |
| **Focus**                    | Checks the **process**: Are we building the product **right**?                                             | Checks the **product**: Are we building the **right** product?                                       |
| **When Performed**           | Conducted at **every stage** of development (design, coding, etc.).                                        | Conducted at the **end** of a module or after the product is fully built.                            |
| **Examples**                 | Code reviews, walkthroughs, inspections, requirements analysis, and design validation.                    | Unit tests, integration tests, system tests, and User Acceptance Tests (UAT).                        |
| **Documents Reviewed**       | Requirements specifications, design blueprints, ER diagrams, test cases, traceability matrix, etc.         | Final product deliverables and customer requirements documents.                                     |
| **Purpose**                  | Ensures the system design and architecture are accurately engineered and error-free.                      | Validates that the product fulfills the true needs and expectations of stakeholders and customers.   |
| **IEEE Definition**          | Involves studying specifications and checking them against code logic.                                    | Defined as ensuring that the product meets stakeholder’s true needs and expectations (IEEE-STD-610). |

---

### **Manual Testing vs. Automated Testing**  

| **Aspect**           | **Manual Testing**                         | **Automated Testing**                     |
|----------------------|--------------------------------------------|-------------------------------------------|
| **Definition**       | Testing without automation tools.          | Testing using specialized tools.          |
| **Human Involvement**| Requires manual effort.                    | Minimal once automated.                   |
| **Knowledge**        | No programming required.                   | Requires programming knowledge.           |
| **Efficiency**       | Time-consuming, error-prone.               | Faster, reliable for repetitive tasks.    |
| **Cost**             | Low upfront, costly over time.             | High upfront, cost-effective long-term.   |
| **Use Cases**        | Best for exploratory or usability testing. | Ideal for regression or performance tests.|

---

![](https://i.ibb.co/t2HkNjG/Untitled.png)

---

### Quality and Reliability in Software

#### **Quality**
- **Definition**: Degree to which a software product conforms to its specifications, requirements, and standards.
- **Measuring Quality**:
  - **Defect Density**: Number of defects per unit of size.
  - **Customer Satisfaction**: Surveys, reviews, ratings, or feedback forms.
  - **Code Coverage**: Percentage of source code tested by a test suite.

#### **Reliability**
- **Definition**: Probability that a software product will perform its intended functions without failure or error under specified conditions and time.
- **Measuring Reliability**:
  - **Failure Rate**: \( \text{Failure Rate} = \frac{\text{Number of Failures}}{\text{Time Period}} \)
  - **Mean Time Between Failures (MTBF)**: Average time between failures.
  - **Mean Time to Repair (MTTR)**: Average time required to repair a failure.
