# 📊 Architectural Diagrams with Mermaid

This folder contains **proven prompts** for generating architectural diagrams using **Mermaid** to visualize system structure and data flow. These prompts help you understand, document, and communicate your system architecture effectively.

## 📦 **What We Created**

### **1. 📖 comprehensive-guide.md** (Full Diagramming Guide)
- **Complete diagramming workflow** from code to visual
- **Multiple diagram types** (flowcharts, sequences, class diagrams)
- **C4-model approach** (start low-level, abstract upward)
- **Best practices** for different scenarios
- **Integration with development workflow**

**Best for:** Complex system documentation, architecture reviews, onboarding materials

### **2. ⚡ quick-prompt.md** (Fast Diagram Generation)
- **Condensed version** for immediate diagram needs
- **Common diagram patterns** ready to use
- **Minimal context** required
- **Perfect for debugging** and quick visualization

**Best for:** Understanding data flow, debugging logic, quick documentation

### **3. 🔧 mermaid-templates.md** (Diagram Templates)
- **Ready-to-use templates** for common scenarios
- **Flowchart, sequence, and class diagram** starters
- **Best practices** built into templates
- **Customizable examples**

**Best for:** Consistent diagram styles, team standards, quick starts

## 🚀 **How to Use These Prompts**

### **Quick Diagram (5 minutes)**
```bash
# 1. Copy the quick prompt
cp .prompts/guides/architectural-diagrams/quick-prompt.md
# 2. Fill in your specific component/flow to diagram
# 3. Paste into AI assistant
```

### **Comprehensive System Documentation (30+ minutes)**
```bash
# 1. Copy the comprehensive guide
cp .prompts/guides/architectural-diagrams/comprehensive-guide.md
# 2. Customize with your system details
# 3. Work through the step-by-step process with AI
```

### **Using Templates**
```bash
# 1. Copy the template file
cp .prompts/guides/architectural-diagrams/mermaid-templates.md
# 2. Choose the appropriate template for your use case
# 3. Customize with your specific components
```

## 📋 **Context Examples**

### **Data Flow Tracing:**
```
System to diagram: User authentication flow from login form to database
Current understanding: I know the frontend and backend, but unclear on middleware
Diagram purpose: Debug why some users can't log in
Output format: Sequence diagram showing each step and potential failure points
```

### **Component Architecture:**
```
System to diagram: Microservices architecture for e-commerce platform
Current understanding: We have 5 services but their interactions are unclear
Diagram purpose: Onboard new team members and plan refactoring
Output format: Component diagram showing services, databases, and data flow
```

### **Logic Flow Understanding:**
```
System to diagram: Order processing pipeline from cart to fulfillment
Current understanding: Code exists but business logic flow is complex
Diagram purpose: Identify optimization opportunities and document process
Output format: Flowchart showing decision points and business rules
```

## 🎯 **Diagram Strategy (Based on C4 Model)**

### **1. Start Small & Specific**
- Pick **one function, route, or process**
- Focus on **detailed, low-level flow**
- Don't try to map everything at once

### **2. Build Upward**
- Create **mid-level component view**
- Combine related flows
- Abstract common patterns

### **3. System-Level View**
- Merge components into **system overview**
- Show **major data flows**
- Highlight **key decision points**

## 📊 **Diagram Types & When to Use**

| Diagram Type | Best For | Mermaid Format |
|--------------|----------|----------------|
| **Flowchart** | Logic flow, decision trees, process flows | `flowchart TD` |
| **Sequence** | API interactions, user flows, time-based processes | `sequenceDiagram` |
| **Class** | Object relationships, data models, inheritance | `classDiagram` |
| **Graph** | Simple directional relationships | `graph TD` |

## 🛠️ **Setup Requirements**

### **Mermaid Extension (Recommended)**
1. Go to Extensions tab in your editor
2. Search for "Mermaid"
3. Install for diagram preview

### **Alternative Tools**
- **Online**: [Mermaid Live Editor](https://mermaid.live/)
- **VS Code**: Mermaid extension
- **Documentation**: Renders automatically in GitHub/GitLab

## ✅ **Success Metrics**

After using these prompts, you should have:
- **Clear visual representation** of your system
- **Better understanding** of data flow and logic
- **Documentation** that helps onboarding
- **Identification** of optimization opportunities
- **Improved communication** about architecture

## 💡 **Best Practices**

1. **Start with purpose**: What question are you trying to answer?
2. **Be specific**: "Show me user login flow" vs "diagram my app"
3. **Iterate**: Start simple, add complexity gradually
4. **Validate**: Does the diagram match your understanding?
5. **Keep updated**: Diagrams should evolve with your code

## 🔗 **Related Resources**

- **Cursor Tutorial**: [Architectural Diagrams](https://docs.cursor.com/guides/tutorials/architectural-diagrams)
- **Mermaid Documentation**: [https://mermaid.js.org/](https://mermaid.js.org/)
- **C4 Model**: [https://c4model.com/](https://c4model.com/)

## ⚠️ **Important Guidelines**

- **Don't guess system details** - ask for clarification when information is missing
- **Stay accurate** - only diagram what you can verify from provided code/context
- **Ask questions** - when system behavior is unclear, ask the user for details
- **Admit limitations** - say "I don't know" rather than making assumptions

---

**Pattern Maturity**: ✅ **Production Ready**  
**Last Updated**: January 2025  
**Maintained By**: Development Team 