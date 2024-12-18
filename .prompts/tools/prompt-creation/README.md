# 🏗️ Prompt Creation Tools

This folder contains **meta-prompts** that help you create new prompts for the team's `.prompts/` collection. These tools assist in extracting, analyzing, and documenting patterns that can benefit the entire team.

## 📦 **What We Created**

### **1. 🏗️ pattern-generator.md** (New Pattern Creator)
- **Input**: An idea, standard, pattern, or reference
- **Output**: Complete folder structure with README, comprehensive guide, quick prompt, and templates
- **Best for**: Creating prompts from scratch, documenting new standards, formalizing team practices

### **2. 🔍 code-analyzer.md** (Pattern Extractor)
- **Input**: Existing code that demonstrates good patterns
- **Output**: Analysis of reusable patterns and corresponding prompt templates
- **Best for**: Extracting wisdom from successful implementations, standardizing proven approaches

### **3. 🦆 rubber-ducky.md** (Problem Solver)
- **Input**: A problem, challenge, or idea you're wrestling with
- **Output**: Conversational guidance through questions and exploration
- **Best for**: Brainstorming solutions, debugging approaches, exploring trade-offs

## 🎯 **When to Use Each Tool**

| Situation | Use This Tool | Example |
|-----------|---------------|---------|
| "I want to standardize our API design process" | **pattern-generator.md** | Create API design pattern prompts |
| "This component architecture works really well" | **code-analyzer.md** | Extract reusable component patterns |
| "I'm stuck on how to handle this use case" | **rubber-ducky.md** | Think through the problem collaboratively |
| "We need better git commit standards" | **pattern-generator.md** | Create git workflow prompts |
| "This error handling approach is solid" | **code-analyzer.md** | Formalize error handling patterns |
| "Should we use library X or Y?" | **rubber-ducky.md** | Explore trade-offs and decision criteria |

## 🚀 **How to Use These Tools**

### **Creating a New Pattern from Scratch**
```bash
# 1. Copy the pattern generator prompt
cp .prompts/tools/prompt-creation/pattern-generator.md

# 2. Fill in your pattern details:
#    - Pattern name/topic
#    - Use cases and target audience
#    - Your team's tech stack and challenges

# 3. Paste into AI assistant and follow the guided process
```

### **Extracting Patterns from Existing Code**
```bash
# 1. Copy the code analyzer prompt  
cp .prompts/tools/prompt-creation/code-analyzer.md

# 2. Add your code and context:
#    - Code type and language
#    - Why this code is worth extracting
#    - Design decisions and trade-offs

# 3. Work with AI to analyze and extract reusable patterns
```

### **Brainstorming and Problem Solving**
```bash
# 1. Copy the rubber ducky prompt
cp .prompts/tools/prompt-creation/rubber-ducky.md

# 2. Fill in your problem context:
#    - What you're working on
#    - Constraints and previous attempts
#    - Desired outcomes

# 3. Have a conversation with AI to explore solutions
```

## 📋 **Quality Checklist for New Prompts**

Before adding a new prompt to the team collection, ensure it meets these criteria:

### **📝 Content Quality**
- [ ] **Clear problem definition**: What specific problem does this solve?
- [ ] **Actionable instructions**: Can someone follow this and get results?
- [ ] **Multiple examples**: Different contexts and use cases covered
- [ ] **Implementation guidance**: Step-by-step instructions included
- [ ] **Error handling**: Common pitfalls and solutions documented

### **🎨 Structure & Style**
- [ ] **Consistent formatting**: Follows team prompt style guidelines
- [ ] **Progressive disclosure**: Quick prompt + comprehensive guide
- [ ] **Visual organization**: Emojis and sections for easy scanning
- [ ] **Copy-paste friendly**: Commands and code blocks ready to use
- [ ] **Context fields**: Customization points clearly marked

### **🔄 Usability**
- [ ] **Self-contained**: All necessary information included
- [ ] **Flexible**: Adaptable to different team contexts
- [ ] **Maintainable**: Easy to update as practices evolve
- [ ] **Tested**: Validated with actual use cases
- [ ] **Documented**: Integration points and dependencies noted

## 💡 **Tips for Successful Prompt Creation**

### **Pattern Discovery**
1. **Look for repetition**: What do you find yourself doing often?
2. **Notice friction**: Where do new team members struggle?
3. **Identify excellence**: What implementations make you say "nice!"?
4. **Document decisions**: What choices required research or debate?

### **Prompt Design**
1. **Start with the end**: What should the AI output look like?
2. **Be specific**: Vague prompts get vague results
3. **Include examples**: Show, don't just tell
4. **Test variations**: Try the prompt with different contexts
5. **Iterate based on feedback**: Improve prompts based on team usage

### **Team Adoption**
1. **Start small**: Create prompts for high-impact, low-complexity patterns
2. **Get buy-in**: Involve team members in prompt creation
3. **Show value**: Demonstrate time savings and quality improvements
4. **Make it easy**: Provide clear usage instructions and examples
5. **Maintain actively**: Keep prompts updated as practices evolve

## 🤝 **Contributing New Meta-Prompts**

Found a gap in our prompt creation tools? Consider adding:

- **Domain-specific generators** (e.g., database schema patterns)
- **Process-focused analyzers** (e.g., workflow optimization)
- **Team collaboration tools** (e.g., architectural decision prompts)
- **Quality assessment helpers** (e.g., code review pattern extractors)

Follow the same pattern: create a clear prompt that helps generate other prompts!

## 🔗 **Related Resources**

- **Main prompts folder**: [../../README.md](../../README.md)
- **Validation pattern example**: [../../patterns/validation/](../../patterns/validation/)
- **Team documentation**: [Refer to your team's development guidelines]

---

**Pattern Maturity**: ✅ **Production Ready**  
**Last Updated**: January 2025  
**Maintained By**: Development Team 