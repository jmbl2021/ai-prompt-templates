# AI Coding Prompt Library

A collection of effective prompts for different stages of AI-assisted development.

---

## REQUIREMENTS & PLANNING PROMPTS

### Research a Domain Before Coding
```
Before we design any solution, I need you to research [DOMAIN] best practices 
for [SPECIFIC PROBLEM].

Please search for:
1. Standard methodologies or frameworks used in this domain
2. Common mistakes or anti-patterns to avoid
3. Key formulas, algorithms, or established approaches
4. Authoritative sources (standards bodies, academic papers, official docs)
5. Real-world examples of how others have solved similar problems

Synthesize what you find and recommend an approach based on established 
best practices, not speculation.
```

**When to use:** Finance, security, healthcare, legal, scientific domains

---

### Request a Design Document (No Code)
```
Before writing ANY code, create a comprehensive design document that includes:

1. **Problem Restatement:** Restate the problem in your own words to confirm 
   understanding

2. **Approach Overview:** High-level strategy for solving this (2-3 sentences)

3. **Data Structures:** What data structures will you use and why?

4. **Algorithm/Logic Flow:** 
   - Pseudocode or step-by-step explanation
   - Key decisions and branch points
   - How you'll handle [SPECIFIC EDGE CASE]

5. **Component Breakdown:** Main functions/classes/modules and their responsibilities

6. **Alternative Approaches:** 
   - What are 2 other ways to solve this?
   - Why did you choose this approach over alternatives?
   - What are the tradeoffs?

7. **Risks & Challenges:** 
   - What's tricky about this problem?
   - What could go wrong?
   - What assumptions are you making?

8. **Example Walkthrough:** Trace through ONE concrete example step-by-step

DO NOT write code yet. I need to review and approve this design first.
```

**When to use:** Any complex project, especially when requirements are unclear

---

### Validate Assumptions
```
Before proceeding, explicitly list ALL assumptions you're making about:

1. **Input Data:**
   - Format, structure, encoding
   - Data quality and consistency
   - Volume and frequency
   - What happens if data is malformed?

2. **My Requirements:**
   - What you think I want vs. what I asked for
   - Implicit requirements you're inferring
   - Success criteria

3. **Technical Environment:**
   - OS, language version, available libraries
   - Performance constraints
   - Deployment context

4. **My Expertise:**
   - What do you assume I understand?
   - What terms might need explanation?

5. **Usage Context:**
   - How will this be used?
   - How often?
   - By whom?

Let me validate or correct these assumptions before you design the solution.
```

**When to use:** After initial requirements discussion, before planning

---

### Red Team My Requirements
```
I've provided requirements for [PROJECT]. Before we start, I want you to 
critique them:

1. **Ambiguities:** What's unclear or could be interpreted multiple ways?

2. **Missing Information:** What critical information haven't I provided?

3. **Contradictions:** Are any requirements contradictory or conflicting?

4. **Edge Cases:** What scenarios haven't I considered?

5. **Unrealistic Expectations:** Is anything here infeasible or overly complex?

6. **Simpler Alternatives:** Is there a much simpler way to achieve my goal?

Be brutally honest. I'd rather fix issues now than after code is written.
```

**When to use:** After drafting requirements, before planning

---

## INCREMENTAL DEVELOPMENT PROMPTS

### Request Proof of Concept
```
Let's start with a minimal proof of concept that demonstrates ONLY the core 
logic with simple, fake data.

For this POC, SKIP:
- Input validation and error handling
- Edge case handling
- User interface or formatting
- Optimization and efficiency
- Documentation and comments
- Production-ready features

FOCUS ONLY ON:
- The core algorithm working with happy-path data
- Demonstrating the approach is sound
- Something I can run and test in 5 minutes

Once this POC works, we'll expand it. But right now, simplest possible 
implementation.
```

**When to use:** Complex projects, uncertain approaches, learning new domains

---

### Iterate from POC to Full Solution
```
The proof of concept works and validates the approach. Now expand it to 
production quality:

Phase 1 - Core Functionality:
- Handle all input scenarios from requirements
- Add proper error handling and validation
- Handle edge cases: [LIST SPECIFIC CASES]

Phase 2 - Polish:
- Add [SPECIFIC FEATURES]
- Optimize for performance
- Add user-friendly error messages
- Add logging/debugging capabilities

Build Phase 1 first. Once that works, we'll do Phase 2.
```

**When to use:** After POC validation, building toward production

---

### Debug Systematically
```
[CODE/ERROR] isn't working as expected. Let's debug systematically:

1. **Reproduce:** Create minimal example that demonstrates the issue

2. **Isolate:** Which specific function/component is causing the problem?

3. **Hypothesis:** What do you think is wrong and why?

4. **Test Hypothesis:** How can we verify that's the issue?

5. **Fix:** Implement fix with explanation

6. **Verify:** Confirm fix works and doesn't break other things

Don't just give me a corrected version. Walk through the debugging process.
```

**When to use:** When code doesn't work and you want to understand why

---

## UNDERSTANDING & VALIDATION PROMPTS

### Explain Like I'm Not Technical
```
Explain how this solution works as if I have no programming background. 

Walk through a concrete example:
- Start with this input: [SPECIFIC DATA]
- Step-by-step, what happens?
- What's the output and why?

Use plain language, no jargon. Focus on the LOGIC, not the code syntax.
```

**When to use:** After receiving a solution, to verify understanding

---

### Justify Technical Decisions
```
For this solution, justify your key technical decisions:

1. **Why [TECHNOLOGY/LIBRARY/APPROACH]?** What alternatives exist and why 
   didn't you choose them?

2. **Why this data structure?** What are the time/space tradeoffs?

3. **Why this algorithm?** What's the complexity? Could we do better?

4. **Why this architecture?** How does it scale? What are the maintenance 
   implications?

For each decision, explain: pros, cons, and what would make you choose 
differently.
```

**When to use:** Complex projects, learning, when decisions seem arbitrary

---

### Test My Understanding
```
I'm going to explain how I think this code works. Correct any 
misunderstandings:

[YOUR EXPLANATION]

Tell me:
1. What did I get right?
2. What did I misunderstand?
3. What important details did I miss?
```

**When to use:** Before finalizing code, to verify comprehension

---

## DOCUMENTATION PROMPTS

### Request Comprehensive Documentation
```
Create comprehensive documentation for this solution:

1. **Overview:** What does this do? Why does it exist?

2. **Setup:**
   - Installation/dependencies
   - Configuration required
   - How to run it

3. **Usage Examples:** 5 concrete examples showing:
   - Basic usage
   - Common scenarios
   - Edge cases
   - Error handling

4. **Input/Output Specifications:**
   - Detailed format descriptions
   - Valid ranges and constraints
   - Examples of good and bad inputs

5. **How It Works:**
   - High-level algorithm explanation
   - Why key design decisions were made
   - Diagrams if helpful

6. **Limitations & Gotchas:**
   - What doesn't this handle?
   - What should users be careful about?
   - Known issues or workarounds

7. **Maintenance Guide:**
   - How to modify or extend this
   - Where to look for different functionality
   - Common modification scenarios

8. **Troubleshooting:**
   - Common errors and solutions
   - How to debug issues
   - Where to get help

Write for someone who might use or maintain this in 6 months with no context.
```

**When to use:** After code works, before considering project complete

---

### Create Inline Comments
```
Add detailed inline comments to this code following these rules:

1. **Why, not What:** Explain WHY decisions were made, not just what the 
   code does

2. **Tricky Parts:** Any non-obvious logic, edge cases, or gotchas

3. **Examples:** For complex functions, show example input/output in comments

4. **Warnings:** Things that could break if modified incorrectly

5. **TODOs:** Known limitations or future improvements

6. **Citations:** If based on algorithm/formula, cite the source

Don't over-comment obvious code. Focus on places where future maintainers 
will say "why did they do it this way?"
```

**When to use:** Before committing code, especially for complex logic

---

## OPTIMIZATION & REFACTORING PROMPTS

### Performance Analysis
```
Analyze the performance of this solution:

1. **Time Complexity:** Big-O for each major operation

2. **Space Complexity:** Memory usage and scalability

3. **Bottlenecks:** Where would this get slow? At what scale?

4. **Optimization Opportunities:** 
   - What could be faster?
   - What's the tradeoff?
   - When would optimization matter?

5. **Recommendation:** Given [EXPECTED USAGE], is this performant enough 
   or should we optimize?

Don't optimize prematurely. Tell me if it's good enough as-is.
```

**When to use:** When performance matters, after core functionality works

---

### Refactor for Clarity
```
This code works but is hard to understand. Refactor it to be more readable:

Goals:
1. Clear variable and function names
2. Single responsibility per function
3. Eliminate magic numbers/strings
4. Add helpful comments
5. Simplify complex conditionals
6. Extract repeated logic

Maintain the same functionality. Explain what you changed and why.
```

**When to use:** When code works but is messy or hard to maintain

---

### Security Review
```
Review this code for security vulnerabilities:

1. **Input Validation:** Are all inputs properly validated and sanitized?

2. **Injection Risks:** SQL, command, code injection possible?

3. **Authentication/Authorization:** Are access controls correct?

4. **Data Exposure:** Is sensitive data properly protected?

5. **Error Handling:** Do errors leak sensitive information?

6. **Dependencies:** Are there known vulnerabilities in libraries?

7. **Best Practices:** Are we following security standards for [DOMAIN]?

For each issue, explain: risk level, attack scenario, and how to fix.
```

**When to use:** Before deploying anything handling sensitive data

---

## ADVANCED PROMPTS

### Compare Multiple Approaches
```
Show me 3 different ways to solve [PROBLEM], each optimizing for different goals:

**Approach 1: Simplicity**
- Easiest to understand and maintain
- May sacrifice performance

**Approach 2: Performance**
- Fastest/most efficient
- May be more complex

**Approach 3: Flexibility**
- Easiest to modify and extend
- May require more upfront work

For each, provide:
- Pseudocode or high-level description
- Pros and cons
- When you'd choose this approach
- Rough complexity analysis

Don't write full implementations yet. Help me choose the right approach first.
```

**When to use:** Important decisions, learning, architectural choices

---

### Generate Test Cases
```
Generate comprehensive test cases for [FUNCTION/MODULE]:

1. **Happy Path:** Normal, expected inputs

2. **Boundary Conditions:** Min/max values, empty inputs, single elements

3. **Edge Cases:** Unusual but valid inputs

4. **Error Cases:** Invalid inputs that should be rejected

5. **Integration Tests:** How this interacts with other components

For each test:
- Input
- Expected output
- Why this test matters

Format as runnable test code in [TESTING FRAMEWORK].
```

**When to use:** After implementation, before considering code complete

---

## PROMPT TEMPLATE

When creating custom prompts, use this structure:

```
[CONTEXT: What you're trying to accomplish]

[SPECIFIC REQUEST: Exactly what you want]

[CONSTRAINTS: What NOT to do, limitations]

[FORMAT: How you want the response structured]

[EXAMPLE: Concrete example if helpful]

[VERIFICATION: How you'll know if it worked]
```

---

## PROMPT ANTI-PATTERNS (Avoid These)

❌ **Too Vague:**
"Make this better"
"Fix the bug"
"Optimize this"

✅ **Better:**
"Refactor this function to improve readability. Focus on extracting repeated 
logic into helper functions and making variable names more descriptive."

---

❌ **Assuming Context:**
"Implement the feature we discussed"
"Use the usual approach"

✅ **Better:**
"Implement user authentication using JWT tokens as we specified in the 
requirements doc, with email/password login and token refresh."

---

❌ **All at Once:**
"Build the entire application with all features, error handling, tests, 
documentation, and deployment."

✅ **Better:**
"Let's build incrementally. First, create a proof of concept that demonstrates 
the core user flow with fake data. Once that works, we'll add real data handling."

---

❌ **No Examples:**
"Parse this data format"
"Handle these cases"

✅ **Better:**
"Parse this JSON format: [EXAMPLE]. Handle these cases: 1) Missing fields → 
use defaults 2) Invalid types → reject with error message 3) Extra fields → 
ignore them"
