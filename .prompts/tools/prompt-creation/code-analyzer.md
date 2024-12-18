# 🔍 Code Pattern Analyzer & Prompt Extractor

I need you to analyze the code I'm providing and extract reusable patterns that
can become part of our team's `.prompts/` collection. Your job is to identify
the underlying patterns, best practices, and approaches that could benefit other
team members.

## 🎯 **Your Task**

Analyze the provided code and:

1. **Identify patterns** and architectural decisions worth replicating
2. **Extract best practices** that should be standardized
3. **Document the approach** in a way that's teachable to AI assistants
4. **Create prompt templates** that encode this knowledge
5. **Suggest folder structure** for the new pattern

## 📋 **Code Information**

**Code Type:** [DESCRIBE WHAT YOU'RE PROVIDING - e.g., "React component", "API
endpoint", "Database schema", "Build configuration", "Test setup"]

**Language/Framework:** [SPECIFY TECH - e.g., "TypeScript + React", "Node.js +
Express", "Python + FastAPI"]

**Problem Domain:** [WHAT IT SOLVES - e.g., "Form validation", "Authentication
flow", "Data fetching", "Error handling"]

**Why This Code:** [WHY IT'S WORTH EXTRACTING - e.g., "Solved complex validation
issues", "Great error handling", "Excellent performance", "Clean architecture"]

## 💻 **Code to Analyze**

```[language]
[PASTE YOUR CODE HERE]
```

**Additional Context:**

- **File structure**: [DESCRIBE THE BROADER CONTEXT]
- **Dependencies used**: [LIST KEY LIBRARIES/TOOLS]
- **Design decisions**: [EXPLAIN ANY NON-OBVIOUS CHOICES]
- **Trade-offs made**: [WHAT WAS SACRIFICED FOR WHAT BENEFIT]

## 🔍 **Analysis Framework**

Please analyze the code through these lenses:

### **1. Pattern Identification**

- What **architectural patterns** are used?
- What **design principles** are followed?
- What **conventions** are established?
- What **abstractions** are created?

### **2. Reusability Assessment**

- Which parts are **domain-specific** vs **generally applicable**?
- What would need to be **parameterized** for reuse?
- What **dependencies** would need to be documented?
- What **variations** might teams need?

### **3. Teaching Potential**

- What **concepts** would developers need to understand?
- What **common mistakes** does this code avoid?
- What **gotchas** or **edge cases** are handled?
- What **alternatives** were rejected and why?

### **4. Implementation Complexity**

- What's the **learning curve** for this approach?
- What **setup/configuration** is required?
- What **testing strategy** is needed?
- What **maintenance considerations** exist?

## 📝 **Expected Analysis Output**

Please provide:

### **1. Pattern Summary**

- **Pattern name** and brief description
- **Core problem** it solves
- **Key benefits** and trade-offs
- **When to use** vs when not to use

### **2. Extracted Principles**

- **Design principles** demonstrated
- **Best practices** encoded
- **Anti-patterns** avoided
- **Performance considerations**

### **3. Prompt Pattern Recommendation**

- **Suggested category** (tools, patterns, processes, guides)
- **Suggested folder name** for `.prompts/[category]/`
- **Target audience** and complexity level
- **Integration points** with existing patterns

### **4. Prompt Templates (Draft)**

- **Comprehensive guide** structure
- **Quick prompt** outline
- **Key customization points**
- **Template files** needed

### **5. Implementation Guide**

- **Prerequisites** and dependencies
- **Step-by-step** implementation approach
- **Testing/validation** strategy
- **Common pitfalls** and solutions

## 🎨 **Documentation Style**

Follow our team prompt style:

- ✅ Use emojis for visual organization
- ✅ Include practical code examples
- ✅ Provide multiple use case scenarios
- ✅ Add implementation checklists
- ✅ Include troubleshooting tips

## 🔄 **Iterative Process**

**Start by providing your initial analysis** of the pattern and its potential.
Then ask me:

1. **Clarifying questions** about the code's context
2. **Validation questions** about the pattern's applicability
3. **Scope questions** about what aspects to emphasize
4. **Usage questions** about how the team would apply it

This will help ensure the final prompt pattern is **maximally useful** for our
specific team context.

## 💡 **Additional Context**

**Our current prompts:**

- patterns/validation (Zod/TypeScript validation)
- tools/prompt-creation (Meta-prompts for generating new prompts)

**Team context:** [DESCRIBE YOUR TEAM - size, experience level, tech stack,
common challenges]

**Common pain points:** [WHAT PROBLEMS KEEP RECURRING - e.g., "Inconsistent
error handling", "Complex state management", "Slow builds"]

**Success criteria:** [HOW TO MEASURE SUCCESS - e.g., "Reduced bugs", "Faster
development", "Better code reviews"]

---

**Begin by analyzing the code and sharing your initial observations about the
patterns worth extracting!**
