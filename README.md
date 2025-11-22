# AI Coding Templates & Best Practices

This repository contains templates and checklists for effective AI-assisted software development.

## 📁 Files in This Repository

### 1. **project_requirements_template.md**
Comprehensive template for documenting project requirements before starting any coding.

**Use this when:** Starting a new project, regardless of complexity.

**Key sections:**
- Project overview and success criteria
- Functional and non-functional requirements
- Data specifications (inputs/outputs)
- Business logic and workflow
- Technical specifications
- Testing scenarios
- Examples and edge cases

### 2. **ai_coding_project_checklist.md**
Step-by-step checklist to follow during AI-assisted development projects.

**Use this when:** Working on any coding project with an AI assistant.

**Phases covered:**
1. Requirements (before any code)
2. Planning (design document)
3. Implementation (POC → full solution)
4. Validation (testing and review)
5. Documentation
6. Post-project reflection

### 3. **ai_coding_prompt_library.md**
Collection of proven prompts for different development scenarios.

**Use this when:** You need the right prompt for a specific situation.

**Categories:**
- Requirements & planning prompts
- Incremental development prompts
- Understanding & validation prompts
- Documentation prompts
- Optimization & refactoring prompts
- Advanced scenario prompts

## 🚀 Quick Start

### For a New Project

1. **Copy `project_requirements_template.md`** and fill it out
   - Be specific with examples
   - Include sample data
   - Define success criteria

2. **Open `ai_coding_project_checklist.md`** and follow Phase 1
   - Complete requirements checklist
   - Check if domain research is needed
   - Verify requirements completeness

3. **Use prompts from `ai_coding_prompt_library.md`**
   - Start with "Request a Design Document" prompt
   - Use "Validate Assumptions" prompt
   - Request proof of concept before full implementation

4. **Follow the checklist through all phases**
   - Don't skip ahead to implementation
   - Validate at each checkpoint
   - Document lessons learned

### For an Existing Project

1. **If stuck or confused:**
   - Use "Red Team My Requirements" prompt
   - Request "Explain Like I'm Not Technical"
   - Use "Debug Systematically" prompt

2. **If code works but needs improvement:**
   - Use "Refactor for Clarity" prompt
   - Request "Performance Analysis"
   - Run "Security Review" if handling sensitive data

3. **Before finalizing:**
   - Use "Request Comprehensive Documentation" prompt
   - Generate test cases
   - Complete post-project reflection in checklist

## 🎯 Core Philosophy

### The Three Pillars

1. **Plan Before Code**
   - Always request a design document first
   - Review logic in plain language
   - Validate assumptions explicitly

2. **Research Before Design**
   - For specialized domains, research first
   - Use established methodologies
   - Don't reinvent the wheel

3. **Build Incrementally**
   - Start with proof of concept
   - Validate core logic first
   - Add features iteratively

### When to Use External Research

Request domain research if your project involves:
- ✅ Finance (investments, loans, tax, accounting)
- ✅ Healthcare (medical, insurance, compliance)
- ✅ Security (cryptography, authentication, access control)
- ✅ Legal (regulations, contracts, compliance)
- ✅ Scientific (physics, chemistry, statistics, algorithms)
- ✅ Any specialized field with established best practices

**Prompt to use:**
```
Before we design any solution, research [DOMAIN] best practices for 
[PROBLEM]. I want to use established methodologies, not speculation.
```

## 📋 Checklists Reference

### Before Writing ANY Code

- [ ] Requirements template filled out
- [ ] Domain research completed (if applicable)
- [ ] Design document reviewed and approved
- [ ] Assumptions validated
- [ ] Success criteria defined

### Before Considering Project Complete

- [ ] All test scenarios pass
- [ ] Code is documented (inline and external)
- [ ] Logic is understandable
- [ ] Edge cases are handled
- [ ] Performance is acceptable
- [ ] Security is reviewed (if applicable)
- [ ] Post-project reflection completed

## 🎓 Learning from This Project

### What the Mortgage Recast Project Taught Us

**Initial Mistakes:**
1. Jumped to implementation without understanding domain
2. Didn't validate the core question being asked
3. Assumed understanding of "recast" without research
4. Built features before core logic was correct

**What Fixed It:**
1. ✅ Requested external research on recast strategies
2. ✅ Asked for planning document before code
3. ✅ Critically questioned if the logic answered the right question
4. ✅ Validated understanding at each step

**Key Insight:** The most important question isn't "how do I build this?" 
It's "am I building the right thing?"

## 🔄 Workflow Diagram

```
┌─────────────────────────────────────────────────────────────┐
│ REQUIREMENTS                                                 │
│ - Fill template                                              │
│ - Check domain research trigger                             │
│ - Validate completeness                                     │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ RESEARCH (if specialized domain)                            │
│ - Request domain research                                   │
│ - Review best practices                                     │
│ - Identify established frameworks                           │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ PLANNING                                                     │
│ - Request design document (NO CODE)                         │
│ - Review approach and logic                                 │
│ - Validate assumptions                                      │
│ - Red team requirements                                     │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ PROOF OF CONCEPT                                            │
│ - Build minimal working example                             │
│ - Test core logic only                                      │
│ - Validate approach before scaling                          │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ FULL IMPLEMENTATION                                          │
│ - Expand from POC                                           │
│ - Add error handling                                        │
│ - Handle edge cases                                         │
│ - Add features incrementally                                │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ VALIDATION                                                   │
│ - Test with real data                                       │
│ - Verify understanding                                      │
│ - Review code quality                                       │
│ - Check documentation                                       │
└────────────────────┬────────────────────────────────────────┘
                     │
                     ▼
┌─────────────────────────────────────────────────────────────┐
│ REFLECTION                                                   │
│ - Document lessons learned                                  │
│ - Update templates                                          │
│ - Note effective prompts                                    │
└─────────────────────────────────────────────────────────────┘
```

## 💡 Pro Tips

### 1. **Use the Templates Every Time**
Even for "simple" projects. The discipline pays off when projects grow.

### 2. **Always Start with Research for Specialized Domains**
5 minutes of research can save hours of rework.

### 3. **No Code Before Design**
If you're tempted to skip the planning phase, that's when you need it most.

### 4. **Test Your Understanding**
If you can't explain the logic in plain language, you don't understand it well enough.

### 5. **Build Small, Validate Often**
POC → Test → Expand → Test → Polish → Test

### 6. **Document as You Go**
Don't leave documentation for the end. You'll forget the "why" behind decisions.

### 7. **Keep a Prompt Journal**
Track which prompts worked well for which situations. Build your own library.

## 📝 Memory Update for AI Assistants

When starting a new project with an AI assistant, share this message:

```
I have templates and best practices for AI-assisted coding that I follow.
Before we start ANY coding project, please remind me to:

1. Fill out my requirements template first
2. Check if domain research is needed for specialized topics
3. Request a planning/design document before any code
4. Start with a proof of concept to validate the approach
5. Build incrementally with validation checkpoints

If I skip these steps, please remind me that I have a checklist and 
templates to follow. My templates are in my Git repo at [YOUR_REPO_PATH].

Red flags that should trigger you to pause and ask questions:
- I'm using domain jargon without defining it clearly
- Requirements seem incomplete or contradictory
- I'm asking for many features at once without a plan
- The problem domain is specialized (finance, security, healthcare, etc.)
- I haven't specified success criteria or key metrics
- I'm jumping straight to "write code for X" without planning

In these cases, prompt me to slow down and follow my templates first.
```

## 🔗 Related Resources

- [Anthropic Prompt Engineering Guide](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview)
- [Software Requirements Specification (IEEE)](https://standards.ieee.org/ieee/29148/6937/)
- [Test-Driven Development Methodology](https://martinfowler.com/bliki/TestDrivenDevelopment.html)

## 📌 Version History

- **v1.0** (2025-11-22): Initial template set based on mortgage recast project lessons
  - Project requirements template
  - AI coding checklist
  - Prompt library
  - This README

---

## 🤝 Contributing

This is a living document. After each project, update:
1. Add new effective prompts to the library
2. Update checklist with new lessons
3. Refine requirements template based on what worked
4. Document common pitfalls in README

**Keep the cycle going:** Learn → Document → Apply → Improve
