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
