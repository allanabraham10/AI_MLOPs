# Predict Survivability for the Titanic Dataset using Modular Approach

## TITLE: Transitioning from Research to Production Environment

### LEARNING OBJECTIVES:
At the end of the experiment, you will be able to transition from the research environment to the
production environment. You will understand the concept of modularization and convert the
model developed in Jupyter Notebook into different modules tailored to specific functionalities:
Data Manager, Training, Pipeline, Predict, etc.
You will be able to understand and implement the following aspects:
1. VS code setup and understanding interface components
2. Creating virtual environment, installing requirement, running .py & .ipynb file
3. Understanding __name__ == “__main__” and building our own modules
4. Modularization: Converting a ML model from research environment format (Notebook)
to product environment format (.py files)
A) Creating different modules specific to functionality: Data Manager, Training,
Pipeline, Predict
B) Understanding folder structure
C) Separating configuration files
D) Concept of YAML file

### INTRODUCTION:
What is a production code?
Production code is designed to be deployed to end users as opposed to research code,
which is for experimentation, and building proof of concepts, and research code tends to
be more short-term in nature.
The following are considerations with production code:
- Testability and maintainability: Dividing code into modules that are more
extensible and easier to maintain & test.
- Separating configuration from code where possible, and ensuring that functionality
is tested and documented.
- May need to refactor inefficient parts of the code base and finally, reproducibility.
- Ensuring version control with clear processes for tracking releases and release
versions, requirements, a mark of which dependencies and which versions are used
by the code.
- Ensure that code adheres to standards like PEP8 so that it's easy for others to read
and work.
- Scalability and performance are also important areas to consider: The production
code needs to be ready to be deployed to infrastructure that can be scaled.In modern web applications, this typically means containerization for vertical or
horizontal scaling.

### Testing
Software testing is a crucial part of the software development process. It
involves executing a program or system with the intention of finding errors or verifying
its compliance with specified requirements. The goal of testing is to identify defects and
ensure that the software functions as intended, meet user expectations, and operates
reliably in various scenarios.
Testing provides several benefits to software development:
(i) Error Detection: Testing helps identify bugs, errors, and unexpected behavior in the
software (ii) Verification and Validation: Testing validates that the software meets the
specified requirements and performs as expected. Verification involves checking if the
software conforms to the design and development specifications, while validation
ensures that it meets the user's needs (iii) Risk Mitigation: Testing helps mitigate risks
associated with software failure. By uncovering and fixing bugs early in the development
cycle, potential risks such as system crashes, data loss, security vulnerabilities, or
financial losses can be minimized (iv) Code Maintenance and Refactoring: Testing
facilitates code maintenance and refactoring. When tests are in place, developers can
confidently modify or refactor existing code without the fear of introducing new defects.
(v) Documentation and Understanding: Tests serve as executable documentation of
the software's behavior. They help developers understand the codebase better by acting
as living examples and serving as a guide for future development.
Pytest is a popular testing framework in Python that simplifies the process of writing and
executing tests. It provides a clean and concise syntax for defining test cases, fixtures
for test setup and teardown, test discovery, and powerful assertions. Pytest integrates well with other tools and frameworks, making it a valuable tool for boosting testing
productivity.

Types of Tests: 
Three types of tests can be designed: Unit test, Integration test
and system test. A unit test is the smallest and simplest form of software testing.
These tests are employed to assess a separable unit of software such as a class or a
function for correctness, independent of the larger software system composed of many
such unit components. A unit test verifies and passes individual units which are
assembled into larger components. The integration tests are run on an assembled
component to verify that it functions correctly, and finally, the system tests cover the
end-to-end functionality of the system.
How much should we test? Prioritizing test for code base - functions or classes that are
absolutely mission critical. This reduces uncertainty about the system's functionality
when there is any change in the system.
Testing design for machine learning systems is complex as compared to a
traditional software system. The system behavior is controlled by software code
only in a traditional software system. The ML model and the data are additional
new elements in machine learning systems, which impact the behavior of the ML
system

### Package
A package is a collection of Python modules, and it is a useful way for us to publish
related functionality so that different project applications can install our package and
make use of the Python modules. The files that are related to packaging are
pyproject.toml, setup.py, manifest.in and mypy.ini file.
