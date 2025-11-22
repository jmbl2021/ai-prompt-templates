# Project Requirements Template

**Project Name:** [Descriptive name]  
**Date:** [YYYY-MM-DD]  
**Status:** [Planning / In Progress / Complete]

---

## 1. PROJECT OVERVIEW

### Purpose
<!-- Why does this project exist? What problem does it solve? -->

### Context
<!-- What background information is important? -->
<!-- What's the current situation that led to this need? -->

### Success Criteria
<!-- How will you know this project succeeded? -->
<!-- What specific outcomes matter? -->

---

## 2. REQUIREMENTS SPECIFICATION

### Functional Requirements
<!-- What must this solution DO? -->

**FR1:** [Description]
- Input: [What goes in]
- Process: [What happens]
- Output: [What comes out]
- Example: [Concrete example with sample data]

**FR2:** [Description]
- Input:
- Process:
- Output:
- Example:

### Non-Functional Requirements
<!-- How should it perform? -->

- **Performance:** [Speed, scale, efficiency requirements]
- **Usability:** [User experience, ease of use]
- **Reliability:** [Error handling, data validation]
- **Maintainability:** [Documentation, code clarity]

---

## 3. DATA SPECIFICATIONS

### Inputs

**Input 1:** [Name]
- **Format:** [File type, data structure, schema]
- **Source:** [Where does it come from?]
- **Sample:** 
```
[Example data]
```
- **Constraints:** [Required fields, data types, valid ranges]
- **Volume:** [How much data? How often?]

**Input 2:** [Name]
[Repeat above structure]

### Outputs

**Output 1:** [Name]
- **Format:** [File type, data structure]
- **Contents:** [What information does it contain?]
- **Sample:**
```
[Example output]
```
- **Success Metrics:** [How to validate it's correct]

---

## 4. BUSINESS LOGIC & WORKFLOW

### Core Logic
<!-- Describe the main algorithm/process in plain language -->

**Step 1:** [What happens first]
- Input: [What's needed]
- Process: [What's done]
- Output: [What's produced]
- Edge cases: [What if...?]

**Step 2:** [What happens next]
[Repeat structure]

### Decision Points
<!-- When does the logic branch? -->

**Decision 1:** IF [condition] THEN [action] ELSE [alternative]
- Example scenario:

**Decision 2:** 
[Repeat structure]

### Calculations/Formulas
<!-- Any specific math or formulas? -->

**Formula 1:** [Name]
```
[Mathematical expression or pseudocode]
```
- Variables: [Define each variable]
- Example: [Walk through with numbers]

---

## 5. USER INTERFACE (if applicable)

### Interaction Model
<!-- How does the user interact with this? -->
- [ ] Command-line interface
- [ ] Web interface
- [ ] Desktop application
- [ ] API
- [ ] File-based (input → process → output)
- [ ] Other: [Specify]

### User Workflow
1. User does [action]
2. System responds with [feedback]
3. User sees [result]

---

## 6. CONSTRAINTS & LIMITATIONS

### Must Have
<!-- Non-negotiable requirements -->
- [Constraint 1]
- [Constraint 2]

### Must NOT Have
<!-- Explicitly excluded features/approaches -->
- [Anti-requirement 1]
- [Anti-requirement 2]

### Assumptions
<!-- What are we assuming is true? -->
- [Assumption 1]
- [Assumption 2]

### Out of Scope
<!-- What is deliberately NOT included in this project? -->
- [Out of scope item 1]
- [Out of scope item 2]

---

## 7. TECHNICAL SPECIFICATIONS

### Technology Stack
- **Language:** [Python, JavaScript, etc.]
- **Framework:** [If applicable]
- **Libraries:** [Key dependencies]
- **Environment:** [Where will this run?]

### Technical Constraints
- **Performance:** [Max runtime, memory limits]
- **Compatibility:** [OS, versions, dependencies]
- **Security:** [Authentication, data protection]

---

## 8. TESTING & VALIDATION

### Test Scenarios

**Test Case 1:** [Scenario name]
- **Given:** [Initial conditions]
- **When:** [Action taken]
- **Then:** [Expected result]
- **Test Data:** [Specific inputs to use]

**Test Case 2:**
[Repeat structure]

### Edge Cases
<!-- What unusual situations should be handled? -->
1. [Edge case 1]
   - Expected behavior: [How should it handle this?]
2. [Edge case 2]

### Acceptance Criteria
<!-- What must be true for this to be "done"? -->
- [ ] [Criterion 1]
- [ ] [Criterion 2]
- [ ] [Criterion 3]

---

## 9. EXAMPLES

### Example 1: [Typical Use Case]
**Scenario:** [Describe situation]

**Input:**
```
[Actual sample data]
```

**Process:** [Step-by-step what should happen]

**Expected Output:**
```
[Actual expected result]
```

### Example 2: [Edge Case]
[Repeat structure]

---

## 10. QUESTIONS & UNKNOWNS

### Open Questions
<!-- What do you need to figure out? -->
1. [Question 1]
2. [Question 2]

### Research Needed
<!-- What external information would help? -->
- [ ] [Research topic 1]
- [ ] [Research topic 2]

### Decisions Pending
<!-- What choices need to be made? -->
1. [Decision point 1]
   - Option A: [Pro/Con]
   - Option B: [Pro/Con]

---

## 11. RISKS & MITIGATION

### Technical Risks
1. **Risk:** [What could go wrong?]
   - **Impact:** [How bad would it be?]
   - **Likelihood:** [How likely?]
   - **Mitigation:** [How to prevent or handle it?]

### Complexity Risks
1. **Risk:** [What might be harder than expected?]
   - **Mitigation:** [How to de-risk it?]

---

## CHECKLIST BEFORE STARTING

Before handing this to an AI assistant, verify:

- [ ] Purpose and success criteria are crystal clear
- [ ] All inputs are specified with examples
- [ ] All outputs are specified with examples
- [ ] Core logic is described step-by-step
- [ ] Edge cases are identified
- [ ] At least 2 concrete examples provided
- [ ] Technical constraints are documented
- [ ] Test scenarios are defined
- [ ] Assumptions are explicitly stated
- [ ] Out-of-scope items are listed

---

## NOTES
<!-- Any additional context, links to related documents, etc. -->
