# AI Coding Project Kickoff Checklist

Use this checklist at the start of every coding project with an AI assistant.

---

## PHASE 1: REQUIREMENTS (Before Any Code)

### 1.1 Problem Definition
- [ ] I have filled out the Project Requirements Template
- [ ] The problem statement is clear in 1-2 sentences
- [ ] I can explain WHY this project is needed
- [ ] Success criteria are measurable and specific

### 1.2 Domain Research Trigger Check
**Ask yourself:** Does this project involve specialized knowledge in:
- [ ] Finance (investments, loans, accounting, taxes)
- [ ] Healthcare (medical, insurance, HIPAA)
- [ ] Security (cryptography, access control, compliance)
- [ ] Legal (regulations, contracts, compliance)
- [ ] Scientific (physics, chemistry, statistics)
- [ ] Other specialized domain: _______________

**If YES to any:** Request domain research BEFORE planning the solution.

**Prompt to use:**
```
Before we design the solution, please research best practices for [domain] 
related to [specific problem]. I want to ensure we're using established 
methodologies and not reinventing the wheel. Search for:
1. Standard approaches in this domain
2. Common mistakes or anti-patterns
3. Key formulas, algorithms, or frameworks
4. Authoritative sources or standards
```

### 1.3 Requirements Completeness Check
- [ ] All inputs are specified (format, source, constraints)
- [ ] All outputs are specified (format, contents, success criteria)
- [ ] Core logic is described in step-by-step plain language
- [ ] At least 2 concrete examples with sample data provided
- [ ] Edge cases are identified
- [ ] Technical constraints are documented
- [ ] Assumptions are explicitly stated

**If ANY are unchecked:** Fill in the gaps before proceeding.

---

## PHASE 2: PLANNING (Before Any Code)

### 2.1 Request Planning Document
**Do NOT ask for code yet.** Instead, request a design document.

**Prompt to use:**
```
Before writing any code, please create a detailed plan that explains:

1. **Approach Overview:** How will you solve this problem? What's the 
   high-level strategy?

2. **Data Structures:** What data structures will you use and why?

3. **Algorithm/Logic:** Step-by-step pseudocode or flowchart of the core logic

4. **Key Functions/Components:** What are the main pieces? What does each do?

5. **Edge Case Handling:** How will you handle [specific edge cases from 
   requirements]?

6. **Alternative Approaches:** What are 2 other ways to solve this? Why did 
   you choose this approach over alternatives?

7. **Potential Issues:** What could go wrong? What's tricky about this problem?

DO NOT write actual code yet. I want to review the design first.
```

### 2.2 Review Planning Document
- [ ] The approach makes sense to me
- [ ] I understand the logic in plain language
- [ ] Edge cases are addressed
- [ ] The AI hasn't made incorrect assumptions
- [ ] Technical choices are justified
- [ ] I can spot any red flags or issues

**If unclear:** Ask for clarification or examples before coding.

### 2.3 Validate Assumptions
**Prompt to use:**
```
Before we proceed, list all assumptions you're making about:
1. The data (format, quality, consistency)
2. My use case and goals
3. Technical environment and constraints
4. My level of expertise
5. How I'll use the solution

Let's validate these before you write code.
```

- [ ] All assumptions reviewed
- [ ] Incorrect assumptions corrected
- [ ] New constraints added to requirements if needed

---

## PHASE 3: IMPLEMENTATION

### 3.1 Start with Proof of Concept
**For complex projects, request an MVP first:**

**Prompt to use:**
```
Let's start with a minimal proof of concept that demonstrates the core logic 
with simple, fake data. Skip:
- Error handling
- Edge cases
- User interface polish
- Optimization

I want to validate the approach works before building the full solution.
```

### 3.2 Test the Core Logic
- [ ] Run the POC with test data
- [ ] Verify the logic produces expected results
- [ ] Check that the approach is sound

**If POC fails or doesn't make sense:** Revisit the planning phase.

### 3.3 Iterate to Full Solution
Once POC validated:

**Prompt to use:**
```
The proof of concept works. Now expand it to:
1. Handle all input scenarios from the requirements
2. Include proper error handling
3. Handle the edge cases we identified
4. Add the missing features: [list specific features]

Maintain the same core approach, just make it production-ready.
```

---

## PHASE 4: VALIDATION

### 4.1 Test with Real Scenarios
- [ ] Test with actual data (not fake examples)
- [ ] Test all scenarios from requirements
- [ ] Test edge cases
- [ ] Try to break it

### 4.2 Understanding Check
**Prompt to use:**
```
Explain how this solution works to me as if I'm not technical. Walk through 
what happens step-by-step using a concrete example with real data.
```

- [ ] The explanation makes sense
- [ ] I can follow the logic
- [ ] No mysterious "magic" that I don't understand

### 4.3 Code Review
- [ ] Code is readable and well-commented
- [ ] Variable names are clear
- [ ] Functions have clear single purposes
- [ ] No obvious inefficiencies
- [ ] Follows best practices for the language

---

## PHASE 5: DOCUMENTATION

### 5.1 Request Comprehensive Documentation
**Prompt to use:**
```
Create documentation that includes:

1. **Setup Instructions:** How to install/configure/run this

2. **Usage Examples:** 3-5 concrete examples showing how to use this for 
   different scenarios

3. **Input/Output Specifications:** Detailed format descriptions

4. **Logic Explanation:** How does the core algorithm work? Why did you 
   design it this way?

5. **Limitations & Gotchas:** What doesn't this handle? What should users 
   be careful about?

6. **Troubleshooting:** Common errors and how to fix them

7. **Maintenance Notes:** If I need to modify this later, what should I know?
```

### 5.2 Documentation Checklist
- [ ] Setup instructions are complete
- [ ] Examples are provided with real data
- [ ] Logic is explained (not just "what" but "why")
- [ ] Limitations are documented
- [ ] Future me will understand this in 6 months

---

## RED FLAGS (Pause and Reassess)

Stop and reconsider if:

- [ ] You're not sure if the AI understands the problem
- [ ] The AI made assumptions you didn't explicitly state
- [ ] The solution feels overly complex for a simple problem
- [ ] You can't explain the logic in your own words
- [ ] Testing reveals the logic is fundamentally wrong
- [ ] You're iterating multiple times without getting closer to success
- [ ] The AI is using terminology you don't understand
- [ ] Requirements keep changing as you learn more

**Action:** Go back to requirements phase. Clarify the problem before continuing.

---

## POST-PROJECT REFLECTION

After project completion, document lessons learned:

### What Went Well
- [ ] What requirements/planning techniques worked?
- [ ] What prompts were particularly effective?
- [ ] What decisions saved time?

### What Could Improve
- [ ] What requirements were missing initially?
- [ ] What caused rework or confusion?
- [ ] What would you do differently next time?

### Update Templates
- [ ] Add new insights to this checklist
- [ ] Update requirements template with new sections
- [ ] Document domain-specific patterns learned

---

## QUICK REFERENCE: Key Prompts

**For Planning:**
```
Before writing code, create a detailed design document explaining your 
approach, logic, and key decisions. Don't write code yet.
```

**For Domain Research:**
```
Research [domain] best practices for [problem] before we design the solution. 
Find established methodologies and common patterns.
```

**For Assumption Validation:**
```
List all assumptions you're making. Let's validate them before you code.
```

**For Understanding:**
```
Explain this to me like I'm not technical. Use a concrete example.
```

**For Proof of Concept:**
```
Create a minimal POC with fake data that demonstrates core logic. Skip 
polish and edge cases for now.
```

**For Incremental Development:**
```
Now expand the POC to handle [specific requirements] while maintaining 
the same approach.
```
