# 🤖 Team AI Prompts

This folder contains **curated, reusable prompts** for AI assistants (Claude, ChatGPT, etc.) that help standardize common development patterns and processes across our team.

## 📁 **Folder Structure**

```
.prompts/
├── README.md                    # This file
├── tools/                       # Meta-tools for prompt creation
│   └── prompt-creation/         # Generate new team prompts
├── patterns/                    # Development patterns & practices
│   └── validation/              # TypeScript validation with Zod
├── processes/                   # Workflows & procedures  
│   ├── git-workflow/           (future)
│   └── rfc-templates/          (future)
└── guides/                     # Documentation & standards
    └── api-design/             (future)
```

## 📂 **Category Guide**

### **🛠️ tools/**
Meta-prompts that help you create and improve other prompts.
- **Best for**: Building new team patterns, extracting code wisdom, problem-solving

### **🎯 patterns/**
Development patterns, architectural approaches, and coding standards.
- **Best for**: Code implementation, technical consistency, reusable solutions

### **🔄 processes/**
Workflows, procedures, and team collaboration practices.
- **Best for**: Git workflows, deployment processes, code reviews, documentation

### **📚 guides/**
Documentation standards, style guides, and reference materials.
- **Best for**: API design, writing standards, architectural decisions

## 🎯 **Purpose**

- **Standardize Development Patterns**: Ensure consistent implementation across projects
- **Accelerate Onboarding**: Help new team members learn established patterns quickly
- **Reduce Research Time**: Pre-researched, battle-tested approaches ready to use
- **Maintain Code Quality**: Enforce best practices through AI-assisted development

## 🚀 **How to Use**

### **For Individual Developers:**
1. Browse categories to find relevant patterns or processes
2. Copy the appropriate prompt template
3. Customize the context section with your specific needs
4. Paste into your AI assistant chat

### **For Team Leaders:**
1. Add new proven patterns and processes to appropriate categories
2. Include comprehensive documentation and examples
3. Update this README when adding new prompt collections
4. Share successful implementations with the team

### **When Adding New Prompts:**
1. **Use our prompt creation tools** in `tools/prompt-creation/` to generate these automatically!
2. **Or choose the right category (manual way)** (tools, patterns, processes, guides) - or ask an LLM for the recommended category.
3. Create a descriptive folder name within that category
4. Include these files in each folder:
   - `README.md` - Overview and usage instructions
   - `comprehensive-guide.md` - Detailed implementation guide
   - `quick-prompt.md` - Condensed version for fast use
   - Template files (if applicable)

## 📋 **Available Prompts**

| Category | Prompt Collection | Description | Use Cases |
|----------|------------------|-------------|-----------|
| **🛠️ Tools** | [prompt-creation](./tools/prompt-creation/) | Meta-prompts for creating new team prompts | Generating new patterns, extracting code wisdom, brainstorming solutions |
| **🎯 Patterns** | [validation](./patterns/validation/) | Modern TypeScript validation with Zod | API validation, form handling, data transformation |
| **🎯 Patterns** | [frontend-data-layer](./patterns/frontend-data-layer/) | Complete frontend data layer with React Query | API integration, CRUD operations, caching strategies, type-safe data fetching |
| **📚 Guides** | [architectural-diagrams](./guides/architectural-diagrams/) | Generate Mermaid diagrams for system visualization | Understanding data flow, documenting architecture, debugging logic |

## 🤝 **Contributing Guidelines**

- **Document thoroughly**: Include context, examples, and rationale
- **Test prompts**: Verify they work with different AI assistants
- **Keep updated**: Maintain prompts as best practices evolve
- **Share learnings**: Add lessons learned and common pitfalls
- **Use categories**: Place prompts in the appropriate folder structure

## 💡 **Tips for Effective Prompt Usage**

1. **Customize context**: Always fill in project-specific details
2. **Start specific**: Use detailed prompts for complex implementations
3. **Iterate**: Refine prompts based on AI assistant feedback
4. **Share improvements**: Update prompts when you find better approaches

---

🏴‍☠️ BK

