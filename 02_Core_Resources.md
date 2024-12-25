# 2. Core Project Resources

This section outlines the core documents and resources used to guide AI-assisted development. Understanding these resources is essential for effective collaboration with the AI assistant.

- **Related Sections**:
  - See [AI Communication](./05_AI_Interaction.md#51-communication-best-practices)
  - See [Development Process](./03_Development_Process.md#31-process-overview)
  - See [Documentation Management](./06_Documentation_Management.md#61-documentation-sources)

---

## 2.1. Rules for AI Management

The Rules for AI system uses a dual-management approach to ensure both flexibility and control in AI behavior. This setup allows for collaborative refinement of AI guidelines while maintaining stable operational rules through Cursor's preferences system.

- **Related Sections**:
  - See [Communication Guidelines](./05_AI_Interaction.md#51-communication-best-practices)
  - See [Quality Assurance](./03_Development_Process.md#33-quality-assurance)
  - See [Continuous Improvement](./07_Self_Evaluation.md#71-purpose-and-benefits)

---

## 2.2. Requirements.md

The Requirements.md file serves as the central reference point for all project specifications and technical requirements. This comprehensive document ensures that all development work aligns with the project's goals and maintains consistent standards.

- **Related Sections**:
  - See [Development Process](./03_Development_Process.md#31-process-overview)
  - See [Project Knowledge](./05_AI_Interaction.md#52-session-management)
  - See [Documentation Integration](./06_Documentation_Management.md#62-documentation-integration)

---

## 2.3. Tasks.md

The Tasks.md file functions as the project's dynamic roadmap, tracking both completed and upcoming work. This living document helps maintain clear progress tracking and ensures systematic development approach.

- **Related Sections**:
  - See [Best Practices](./03_Development_Process.md#32-best-practices)
  - See [Prompt Generation](./05_AI_Interaction.md#53-prompt-generation)
  - See [Timestamp Usage](./04_Timestamp_Management.md#44-user-prompting-and-reminders)

---

## 2.4. ChangeLog.md

The ChangeLog.md file serves as the project's historical record, documenting all changes and decisions. This comprehensive log enables traceability and informed decision-making.

- **Related Sections**:
  - See [Timestamp Generation](./04_Timestamp_Management.md#41-timestamp-generation-and-retrieval)
  - See [Documentation Format](./07_Self_Evaluation.md#72-self-evaluation-documentation)
  - See [Documentation Patterns](./06_Documentation_Management.md#63-documentation-usage-patterns)

---

## 2.5. Document Cross-Linking

GitHub supports markdown links between repository files, enabling seamless navigation between project documentation.

- **Related Sections**:
  - See [Documentation Sources](./06_Documentation_Management.md#61-documentation-sources)
  - See [Best Practices](./03_Development_Process.md#32-best-practices)
  - See [Documentation Benefits](./08_Benefits_and_Outcomes.md#822-documentation-benefits)

### 2.5.1. Link Types
- **Repository Links**: Links to other markdown files
  ```markdown
  [Rules for AI](./Rules%20for%20AI.md)
  [Requirements](./Requirements.md)
  [Tasks](./Tasks.md)
  [ChangeLog](./ChangeLog.md)
  ```

- **Section Links**: Links to specific sections within files
  ```markdown
  [Timestamp Rules](./04_Timestamp_Management.md#42-project-requirements)
  [Development Process](./03_Development_Process.md#31-process-overview)
  ```

### 2.5.2. Best Practices
- Use relative paths for repository links
- URL-encode spaces with %20
- Include file extension (.md)
- Use lowercase for anchor links
- Test links after creation

--- 