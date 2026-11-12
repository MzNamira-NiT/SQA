# QA Fundamentals 
 - **What is QA, QC, and software testing?**
   
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
