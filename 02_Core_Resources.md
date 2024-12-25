[← Previous: Introduction](./01_Introduction.md) | [Next: Development Process →](./03_Development_Process.md)

# 2. Core Project Resources

This section outlines the core documents and resources used to guide AI-assisted development. Understanding these resources is essential for effective collaboration and consistent quality.

**Related Sections**:
- See Section 5.1 for applying these resources
- See Section 3.1 for development workflow
- See Section 8.1 for resource benefits

---

## 2.1. Rules for AI Management

The Rules for AI system uses a dual-management approach to ensure both flexibility and control in AI behavior. This setup allows for collaborative refinement of AI guidelines while maintaining stable operational rules through Cursor's preferences system.

**Related Sections**:
- See Section 5.1 for applying these rules in communication
- See Section 7.1 for continuous improvement process
- See Section 3.3 for quality assurance integration

### 2.1.1. Cursor Preferences vs Rules for AI.md
The Rules for AI are managed through two complementary mechanisms:
- **Cursor Preferences**: Contains the active rules that directly guide the AI's behavior
- **Rules for AI.md**: Serves as the editable version of these rules, allowing for collaborative refinement

### 2.1.2. Rules Management Process
- The AI cannot directly edit Cursor's Rules for AI preferences
- Instead, updates are made to the `Rules for AI.md` file
- After review and approval, the contents are manually copied to Cursor's preferences
- This two-step process ensures careful consideration of all rule changes

### 2.1.3. Periodic Review and Improvement
- Regular reviews of the Rules for AI are conducted to:
  - Identify areas for improvement
  - Incorporate lessons learned
  - Enhance AI performance
  - Address any gaps or inefficiencies
- Changes are documented in ChangeLog.md under the "Rules for AI Updates" category

---

## 2.2. Requirements.md

The Requirements.md file serves as the central reference point for all project specifications and technical requirements. This comprehensive document ensures that all development work aligns with the project's goals and maintains consistent standards across all implementations.

**Related Sections**:
- See Section 3.1 for implementing requirements in development
- See Section 5.2 for maintaining project context
- See Section 6.1 for documentation integration

### 2.2.1. Purpose and Usage
- Central reference for project specifications
- Technical requirements documentation
- Standards and guidelines repository
- Implementation alignment guide

### 2.2.2. Content Organization
- Clear section structure
- Detailed specifications
- Technical guidelines
- Implementation notes
- Version tracking
- Change history

### 2.2.3. Maintenance Process
- Regular updates
- Version control
- Change tracking
- Review process
- Quality checks
- Documentation

---

## 2.3. Tasks.md

The Tasks.md file functions as the project's dynamic roadmap, tracking both completed and upcoming work. This living document helps maintain clear progress tracking and ensures systematic development approach through well-organized, hierarchical task management.

**Related Sections**:
- See Section 3.2 for task execution best practices
- See Section 5.3 for task-related prompts
- See Section 4.4 for timestamp usage in tasks

### 2.3.1. Task Organization
- Numbered sections (e.g., 1.0, 2.0)
- Subsections for complex tasks (e.g., 2.1, 2.2)
- Flexible structure for new additions
- Sequential priority arrangement

### 2.3.2. Task Management
- Clear descriptions
- Priority levels
- Dependencies
- Status tracking
- Progress updates
- Completion criteria

### 2.3.3. Progress Tracking
- Regular updates
- Status changes
- Blockers noted
- Dependencies tracked
- Timeline monitoring
- Completion verification

---

## 2.4. ChangeLog.md

The ChangeLog.md file serves as the project's historical record, documenting all changes and decisions. This comprehensive log enables traceability, context preservation, and informed decision-making throughout the project's lifecycle.

**Related Sections**:
- See Section 4.1 for timestamp generation in logs
- See Section 7.2 for self-evaluation documentation
- See Section 5.3 for changelog-related prompts

### 2.4.1. Change Documentation
- Record of all modifications
- Timeline of development activities
- Context and rationale preservation
- Traceability maintenance

### 2.4.2. Entry Format
- Precise timestamps
- Clear descriptions
- Related task references
- Impact assessment
- Version information
- Author attribution

### 2.4.3. Usage Guidelines
- Regular updates
- Consistent format
- Clear references
- Detailed context
- Version tracking
- Change categorization

---

## 2.5. Document Cross-Linking

This section explains how GitHub supports markdown links between repository files and provides examples of repository and section links.

### 2.5.1. Repository Links
- Direct file links: `[Rules for AI](./Rules%20for%20AI.md)`
- Core documents: `[Requirements](./Requirements.md)`, `[Tasks](./Tasks.md)`, `[ChangeLog](./ChangeLog.md)`
- Documentation: `[Cursor Usage](./Cursor%20Usage.md)`

### 2.5.2. Section Links
- Specific sections: `[Timestamp Rules](./Requirements.md#timestamp-rules)`
- Process references: `[Development Process](./Cursor%20Usage.md#3-development-process-and-workflow)`
- Documentation links: `[Documentation Management](./Cursor%20Usage.md#6-documentation-management)`

### 2.5.3. Link Maintenance
- Regular validation
- Path verification
- Section updates
- Format consistency
- Reference checks
- Documentation updates

---

[← Previous: Introduction](./01_Introduction.md) | [Next: Development Process →](./03_Development_Process.md) 