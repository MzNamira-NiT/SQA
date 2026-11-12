# QA Fundamentals 
 ### **What is QA, QC, and software testing?**
   
 | Aspect             | Quality Assurance (QA)                           | Quality Control (QC)                | Software Testing                        |
| ------------------ | ------------------------------------------------ | ----------------------------------- | --------------------------------------- |
| Primary Goal       | Prevent defects                                  | Detect defects                      | Find bugs and verify software behavior  |
| Orientation        | Process-oriented                                 | Product-oriented                    | Product/Execution-oriented              |
| Nature             | Proactive (before/during development)            | Reactive (after/during development) | Practical execution                     |
| Who is Responsible | Entire team (developers, managers, QA engineers) | Specialized reviewers and testers   | Testers, Test Engineers, and Developers |


1. **Quality Assurance (QA)**:
- Definition: A process-oriented, proactive management activity focused on preventing defects before they happen.
- Focus: How the software is built. It establishes the rules, guidelines, workflows, and standards (such as coding standards, review processes, and team training).
- Approach: Preventive. It spans the entire development lifecycle, often involving the entire team rather than just a specialized sub-team.
- Example: Defining coding guidelines, conducting process audits, or setting up a CI/CD pipeline policy.

2. **Quality Control (QC)**:
- Definition: A product-oriented, reactive verification activity focused on finding defects in the actual deliverables.
- Focus: What has been built and whether it complies with specified requirements.
- Approach: Detective. It evaluates the finished or semi-finished product to verify that quality standards set by QA are met.
- Example: Inspecting builds, reviewing design outputs, or running verification checks on a feature branch.

3. **Software Testing** :
- Definition: A core technical subset and mechanism of Quality Control.
- Focus: Executing the software (manually or via automation) to evaluate its behavior, find bugs, and ensure it functions as expected.
- Approach: Involves designing test cases, running functional and non-functional tests (like performance, security, or unit tests), and reporting defects back to developers.
- Example: Running an automated login script or executing a manual test checklist on a mobile payment screen.



### SDLC vs. STLC

| Feature      | SDLC (Software Development Life Cycle)                          | STLC (Software Testing Life Cycle)                                |
| ------------ | --------------------------------------------------------------- | ----------------------------------------------------------------- |
| Scope        | Covers the complete end-to-end journey of software development. | A focused subset dedicated strictly to testing and validation.    |
| Primary Goal | To build and deploy a working software product.                 | To verify quality, find bugs, and ensure reliability.             |
| Primary Team | Developers, product owners, architects, and managers.           | QA engineers, testers, and test leads.                            |
| Team Size    | Typically requires a larger overall team.                       | Typically handled by a smaller, specialized QA team.              |
| Relationship | The overarching framework for software development.             | Integrated directly into SDLC as its quality assurance component. |


### What is SDLC? (Software Development Life Cycle)

SDLC is a structured framework that guides a team through the entire process of conceiving, building, deploying, and maintaining a software application. Its primary goal is to deliver functional software that meets business and user requirements within budget and time limits.

**Core Phases of SDLC**

- Planning / Requirement Analysis: Identifying the project scope, goals, and business/user requirements.
- System Design: Defining the software architecture, database structure, and UI/UX layouts.
- Implementation (Coding): Writing the actual source code for the application.
- Testing: Reviewing code and checking basic functionality (often where QA steps in).
- Deployment: Releasing the software to the live production environment.
- Maintenance: Providing updates, fixing live issues, and supporting users over time.

### What is STLC? (Software Testing Life Cycle)

STLC is a systematic sequence of activities executed by the quality assurance (QA) team to validate software quality and ensure it is defect-free before release. Unlike the popular misconception that testing only begins after coding finishes, STLC starts alongside early requirements analysis.

**Core Phases of STLC**

- Requirement Analysis (Testing Perspective): Reviewing requirements to identify what features need testing and what testability issues exist.
- Test Planning: Defining the testing strategy, test lead responsibilities, tool selection, and resource/time estimates.
- Test Case Development: Writing test scripts, test cases, and creating traceability matrices.
- Test Environment Setup: Configuring the hardware, software, and test data needed to simulate real-world usage.
- Test Execution: Running the test cases, logging bugs, and reporting defects to developers.
- Test Cycle Closure: Evaluating test coverage, summarizing results, and conducting sign-offs.



### Testing principles and testing levels

**The 7 Principles of Software Testing (ISTQB)** :

According to the ISTQB Foundation Level Principles, software testing is guided by seven fundamental principles:
1. Testing shows defect presence, not absence: Testing can prove that defects exist, but it cannot prove that zero defects remain.
2. Exhaustive testing is impossible: Testing every single input combination, path, and pre-condition is unfeasible for anything beyond trivial code; use risk analysis and prioritization instead.
3. Early testing saves time and money: Starting static reviews and dynamic tests early in the software development lifecycle ("shift left") catches expensive flaws sooner.
4. Defects cluster together: A small number of modules or components usually hold most of the system defects (applying the Pareto 80/20 rule).
5. Pesticide paradox: Repeating the exact same test suite over and over eventually stops finding new bugs; test cases must be regularly reviewed and updated.
6. Testing is context-dependent: Testing approaches vary depending on the nature of the application (e.g., medical software vs. an e-commerce website).
7. Absence-of-errors is a fallacy: Fixing all found bugs does not guarantee a usable or successful system if the software fails to meet user business needs.

**The 4 Levels of Software Testing** :

Testing levels define the sequential stages in the Software Development Life Cycle (SDLC) where specific verification tasks take place, moving from isolated components to the whole application:
1. Unit Testing
	- Scope: Individual code units, functions, or classes.
	- Who performs it: Developers.
	- Goal: Verify that each small, isolated piece of logic works as expected.
2. Integration Testing
	- Scope: Combined modules, interfaces, and data flow between components.
	- Who performs it: Developers or testers.
	- Goal: Detect interface defects and communication errors when individual units work together.
3. System Testing
	- Scope: The complete, integrated software product as a whole in an environment mirroring production.
	- Who performs it: Independent quality assurance (QA) or professional testers.
	- Goal: Verify both functional and non-functional requirements (performance, security, usability) across the entire system.
4. Acceptance Testing
	- Scope: Complete end-to-end business workflows and user scenarios.
	- Who performs it: Customers, end users, or product stakeholders.
	- Goal: Confirm that the software satisfies business requirements and is ready for real-world release.

### Manual Testing vs. Automation Testing

| Attribute              | Manual Testing                                                        | Automation Testing                                                     |
| ---------------------- | --------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| Execution              | Performed directly by human testers interacting with the application. | Executed by software tools, frameworks, and scripts.                   |
| Speed                  | Slower; takes hours or days for large test suites.                    | Very fast; runs thousands of checks in minutes.                        |
| Setup & Maintenance    | Low initial setup cost, but high ongoing labor cost per run.          | High upfront setup cost, but low execution cost at scale.              |
| Accuracy & Consistency | Prone to human error and fatigue during repetitive tasks.             | Highly consistent and accurate when running predefined steps.          |
| Flexibility            | High; testers can adapt on the fly and notice subtle UI flaws.        | Low; scripts only check what they are explicitly programmed to verify. |
| Best Use Cases         | Exploratory, usability, ad-hoc, and early-stage feature testing.      | Regression, smoke, load/performance testing, and CI/CD pipelines.      |



### Functional Testing vs. Non-Functional Testing

| Basis           | Functional Testing                                                                    | Non-Functional Testing                                                                  |
| --------------- | ------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| Core Question   | "Does the feature work?" (Pass/Fail)                                                  | "How well does the system work?" (Measured metrics)                                     |
| Focus           | Features, business logic, inputs, and outputs.                                        | Performance, security, usability, reliability, and scalability.                         |
| Based On        | Functional requirements.                                                              | Non-functional requirements (quality attributes).                                       |
| Common Examples | Unit testing, integration testing, system testing, regression testing, smoke testing. | Performance testing, load testing, stress testing, security testing, usability testing. |
| Execution       | Often done earlier in the cycle; can be manual or automated.                          | Usually done after core features work; heavily relies on automation tools.              |
