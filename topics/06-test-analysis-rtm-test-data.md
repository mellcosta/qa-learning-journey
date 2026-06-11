[← Back to Home](../index.md)

---

# Day 6 - Test Analysis, RTM Deep Dive & Test Data Design 🚀

## Overview

On Day 6, the focus moved into the **structural design phase of QA**, where testing is planned at a more technical and traceable level.

This stage emphasizes how requirements are transformed into test conditions, how coverage is guaranteed through RTM, and how test data is prepared before execution begins.

---

## 🔍 Test Analysis (Test Basis) 😢

Test Analysis is the process of reviewing **source requirement documents (Test Basis)** to determine **what needs to be tested**.

The output of this phase is **Test Conditions**, which are high-level statements of “what to test”.

### 📚 Test Basis Sources

| Source Artifact                           | Best Suited For             | What You Extract                           |
| :---------------------------------------- | :-------------------------- | :----------------------------------------- |
| BRS (Business Requirements Specification) | Acceptance & System Testing | Business rules and end-to-end expectations |
| SRS (Software Requirements Specification) | System Testing              | Functional + non-functional requirements   |
| Design Documents                          | Integration Testing         | Module interaction and data flow           |
| User Stories                              | Agile Testing               | Behavior in Given–When–Then format         |

---

### ⚙️ Test Analysis Workflow 😢

1. Gather all requirement artifacts (BRS, SRS, designs, stories)
2. Review for clarity, completeness, and testability
3. Identify test conditions (high-level “what to test”)
4. Prioritize based on risk and business importance
5. Convert conditions into detailed test cases

---

## 🔗 Requirement Traceability Matrix (RTM) Deep Dive 😢

RTM ensures **100% requirement coverage** by mapping requirements to test cases.

### 🎯 Purpose

* Prevent missing requirements
* Ensure full test coverage
* Support audit and compliance
* Link business needs to execution

---

### 🔄 Types of Traceability

* **Forward Traceability:** Requirements → Test Cases
* **Backward Traceability:** Test Cases → Requirements (prevents scope creep)
* **Bi-directional Traceability:** Both directions combined for full validation

---

### 🧩 RTM Mapping Example 😢

In a banking login scenario:

* Requirement **B1** → Login/Logout functionality
* Technical Requirement **T94** → Valid login behavior
* Test Case **TC-1** → Valid login execution

This ensures every requirement is validated and traceable end-to-end.

---

## 🧪 Test Data Generation 😢

Test Data is the **input used during test execution**. It directly affects test accuracy and coverage.

### 📊 Data Types

* **Positive Data:** Valid inputs (expected success)
* **Negative Data:** Invalid inputs (error handling)
* **Boundary Data:** Edge values (min/max limits)
* **Security Data:** Authentication and access control scenarios

---

### ⚙️ Data Generation Methods

* Manual creation (targeted edge cases)
* Mass copy from production (with anonymization)
* Automated generation tools (large datasets)

---

### ⚠️ Key Rule

Test data must be prepared **before execution begins** to avoid delays and incomplete coverage.

---

## 📋 Standard Test Case Templates 😢

Standardization ensures any tester can execute cases without clarification.

### 🧾 Core Fields

| Field           | Description                               |
| :-------------- | :---------------------------------------- |
| Test Case ID    | Unique identifier (e.g., TC_UI_LOGIN_001) |
| Priority        | High / Medium / Low                       |
| Preconditions   | Required system state                     |
| Test Steps      | Step-by-step execution instructions       |
| Test Data       | Input values used                         |
| Expected Result | Desired system behavior                   |
| Actual Result   | Observed system behavior                  |
| Status          | Pass / Fail / Blocked                     |

---

## 🧠 Key QA Insight

This phase introduces **traceability + precision**, where QA work becomes fully structured and auditable.

Key shift:

* From “writing tests”
* To “engineering test systems with full coverage and data control”

---

## ✨ Key Takeaways

1. Test Analysis defines what must be tested before writing cases
2. Test Basis documents drive all QA design decisions
3. RTM ensures full requirement-to-test traceability
4. Traceability prevents missing coverage and scope creep
5. High-quality test data is essential for valid execution
6. Test data must be prepared before execution starts
7. Standardized templates improve consistency and scalability

---

## 💭 Personal Reflection

This stage highlights how QA becomes increasingly structured and systematic.

Instead of focusing only on test execution, the emphasis is now on designing the entire testing architecture in advance.

Understanding RTM and test data design shows how QA ensures not only correctness, but also **completeness and accountability across the system**.

---

## Challenge Progress

**Challenge:** 30-Day QA Learning Challenge

**Day Completed:** Day 6 ✅

---

[← Previous: Day 5](./05-test-documentation-regression.md) | [← Back to Home](../index.md) | [Next: Day 7 →](./07-black-box-testing-techniques.md)
