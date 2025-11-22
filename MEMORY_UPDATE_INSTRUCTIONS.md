# Memory Update Instructions for Claude

Copy and paste this message to Claude at the start of your next session to update memory:

---

Please remember the following preferences for all future coding projects with me:

**My Coding Workflow Preferences:**

1. When I start a coding project, always remind me to:
   - Provide a structured requirements specification before any coding
   - Request domain research for specialized topics (finance, security, healthcare, legal, scientific)
   - Ask for a planning/design document before implementation
   - Build incrementally: proof of concept → core functionality → polish
   - Request explanations of logic in plain language before reviewing code

2. My quality standards:
   - I prefer working code over perfect code
   - I want to understand the logic and reasoning, not just get the solution
   - I value clear documentation that explains WHY decisions were made, not just WHAT the code does
   - I test with real-world scenarios before accepting solutions
   - When I catch errors, acknowledge them and learn from them

3. My development process:
   - Start with requirements template
   - Research phase for domain-specific problems
   - Planning/design review before coding
   - Iterative development with validation checkpoints
   - Final documentation of changes and rationale

4. Red flags that should trigger you to pause and ask questions:
   - I'm using domain-specific terminology without defining it clearly
   - Requirements seem contradictory or incomplete
   - I'm asking for many features at once without a clear plan
   - The problem domain is specialized (finance, security, healthcare, etc.)
   - I haven't specified success criteria or key metrics
   - I'm jumping straight to "write code for X" without discussing approach first

5. When these red flags appear:
   - Remind me that I have templates and checklists in my Git repository
   - Suggest we slow down and clarify requirements first
   - Ask if domain research would be helpful
   - Request that I fill out the requirements template
   - Propose starting with a design discussion instead of code

**Files I Have Available:**
- project_requirements_template.md (for documenting requirements)
- ai_coding_project_checklist.md (step-by-step workflow)
- ai_coding_prompt_library.md (effective prompts for different scenarios)
- README.md (overview and philosophy)

Location: [UPDATE WITH YOUR GIT REPO PATH]

**Important Notes:**
- These templates came from lessons learned on a mortgage recast analysis project
- The key insight: "Am I building the right thing?" matters more than "How do I build this?"
- Three pillars: Plan Before Code, Research Before Design, Build Incrementally

Please apply these preferences to help me maintain good AI-assisted coding practices.

---

## Alternative: Shorter Memory Update

If the above is too long, use this condensed version:

---

For future coding projects, please remind me to follow my templates:

1. Requirements specification before any code
2. Domain research for specialized topics
3. Design document before implementation  
4. Build incrementally with checkpoints
5. Validate understanding at each step

Red flags to watch for:
- Unclear domain terminology
- Incomplete requirements
- Jumping straight to code
- No success criteria defined

When you see these, prompt me to use my templates (in my Git repo at [PATH]).

My philosophy: Plan Before Code, Research Before Design, Build Incrementally.

---
