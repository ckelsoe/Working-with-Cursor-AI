# Cursor Usage Guide

---

## 1. Introduction

### 1.1. Purpose and Scope

This document provides a comprehensive guide for working with Cursor's AI assistant, with a special focus on helping users who are:
- New to AI-assisted development
- Learning to work with Cursor AI for the first time
- Experiencing challenges in their AI collaboration
- Seeking to understand the structured approach to AI-assisted development

- **Related Sections**:
  - See Section 5.1 for communication best practices
  - See Section 8.1 for immediate benefits of this approach
  - See Section 2.1 for Rules for AI overview

### 1.2. Overview

The guide explains how Cursor's AI assistant utilizes various resources to maintain consistent, high-quality development work. It breaks down complex processes into clear, manageable steps and provides practical examples to illustrate key concepts. Whether you're just starting with Cursor or looking to improve your existing workflow, this guide will help you establish effective collaboration with the AI assistant.

- **Related Sections**:
  - See Section 3.1 for development process overview
  - See Section 5.5 for Cursor IDE features
  - See Section 8.2 for project management benefits

## 2. Core Project Resources

### 2.1. Rules for AI Management

The Rules for AI system uses a dual-management approach to ensure both flexibility and control in AI behavior. This setup allows for collaborative refinement of AI guidelines while maintaining stable operational rules through Cursor's preferences system.

- **Related Sections**:
  - See Section 5.1 for applying these rules in communication
  - See Section 7.1 for continuous improvement process
  - See Section 3.3 for quality assurance integration

#### 2.1.1. Cursor Preferences vs Rules for AI.md
The Rules for AI are managed through two complementary mechanisms:
- **Cursor Preferences**: Contains the active rules that directly guide the AI's behavior
- **Rules for AI.md**: Serves as the editable version of these rules, allowing for collaborative refinement

#### 2.1.2. Rules Management Process
- The AI cannot directly edit Cursor's Rules for AI preferences
- Instead, updates are made to the `Rules for AI.md` file
- After review and approval, the contents are manually copied to Cursor's preferences
- This two-step process ensures careful consideration of all rule changes

#### 2.1.3. Periodic Review and Improvement
- Regular reviews of the Rules for AI are conducted to:
  - Identify areas for improvement
  - Incorporate lessons learned
  - Enhance AI performance
  - Address any gaps or inefficiencies
- Changes are documented in ChangeLog.md under the "Rules for AI Updates" category

---

### 2.2. Requirements.md

The Requirements.md file serves as the central reference point for all project specifications and technical requirements. This comprehensive document ensures that all development work aligns with the project's goals and maintains consistent standards across all implementations.

- **Related Sections**:
  - See Section 3.1 for implementing requirements in development
  - See Section 5.2 for maintaining project context
  - See Section 6.1 for documentation integration

#### 2.2.1. Purpose and Usage
- Central reference for project specifications
- Technical requirements documentation
- Standards and guidelines repository
- Implementation alignment guide

---

### 2.3. Tasks.md

The Tasks.md file functions as the project's dynamic roadmap, tracking both completed and upcoming work. This living document helps maintain clear progress tracking and ensures systematic development approach through well-organized, hierarchical task management.

- **Related Sections**:
  - See Section 3.2 for task execution best practices
  - See Section 5.3 for task-related prompts
  - See Section 4.4 for timestamp usage in tasks

#### 2.3.1. Task Organization
- Numbered sections (e.g., 1.0, 2.0)
- Subsections for complex tasks (e.g., 2.1, 2.2)
- Flexible structure for new additions
- Sequential priority arrangement

---

### 2.4. ChangeLog.md

The ChangeLog.md file serves as the project's historical record, documenting all changes and decisions. This comprehensive log enables traceability, context preservation, and informed decision-making throughout the project's lifecycle.

- **Related Sections**:
  - See Section 4.1 for timestamp generation in logs
  - See Section 7.2 for self-evaluation documentation
  - See Section 5.3 for changelog-related prompts

#### 2.4.1. Change Documentation
- Record of all modifications
- Timeline of development activities
- Context and rationale preservation
- Traceability maintenance

---

## 3. Development Process and Workflow

This section outlines the systematic approach that guides all development work. It provides a clear framework for how tasks are analyzed, executed, validated, and documented, ensuring consistent quality and thorough documentation throughout the development lifecycle.

- **Related Sections**:
  - See Section 2.1 for Rules for AI guidelines
  - See Section 5.1 for AI communication practices
  - See Section 8.1 for productivity benefits

---

### 3.1. Process Overview

- **Related Sections**:
  - See Section 2.2 for requirements alignment
  - See Section 4.4 for user prompting guidelines
  - See Section 6.1 for documentation sources

#### 3.1.1. Initial Analysis
The AI begins by:
- Reading the Requirements.md to understand project goals
- Reviewing Tasks.md to identify current objectives
- Checking Rules for AI to ensure compliance

#### 3.1.2. Task Execution
For each task, the AI:
- Analyzes requirements and constraints
- Develops implementation plan
- Executes necessary code changes
- Documents progress in ChangeLog.md

#### 3.1.3. Validation
The AI ensures quality by:
- Verifying changes against requirements
- Running necessary tests
- Updating documentation
- Confirming task completion

#### 3.1.4. Documentation
Throughout the process, the AI:
- Maintains clear records in ChangeLog.md
- Updates task status in Tasks.md
- Provides progress updates to developers
- Suggests improvements when identified

---

### 3.2. Best Practices

- **Related Sections**:
  - See Section 5.1 for communication guidelines
  - See Section 7.1 for continuous improvement
  - See Section 8.2 for organizational benefits

#### 3.2.1. Communication
- Clear and concise explanations
- Professional but accessible language
- Proactive issue identification
- Regular progress updates

#### 3.2.2. Documentation Standards
- Consistent timestamp format
- Detailed change records
- Clear task status updates
- Comprehensive explanations

---

### 3.3. Quality Assurance

- **Related Sections**:
  - See Section 2.2 for requirements validation
  - See Section 5.6 for testing collaboration
  - See Section 7.2 for quality documentation

#### 3.3.1. Testing Procedures
- Regular requirement verification
- Thorough testing procedures
- Consistent code standards
- Proper error handling

#### 3.3.2. Code Quality
- Following established standards
- Implementing best practices
- Maintaining consistency
- Ensuring maintainability

#### 3.3.3. Review Process
- Code review guidelines
- Documentation review
- Quality metrics
- Performance considerations

---

## 4. Timestamp Management

This section explains how timestamps are generated and managed throughout the project lifecycle. It details the hierarchical approach to obtaining accurate timestamps, including primary and fallback methods, and describes how the AI interacts with users to maintain consistent time recording.

- **Related Sections**:
  - See Section 2.3 for timestamp usage in Tasks.md
  - See Section 2.4 for timestamp format in ChangeLog.md
  - See Section 7.2 for timestamps in self-evaluation

---

### 4.1. Timestamp Generation and Retrieval

- **Related Sections**:
  - See Section 5.1 for command execution safety
  - See Section 3.2 for best practices
  - See Section 6.1 for documentation sources

#### 4.1.1. Primary Method
- Requests the user to run the terminal command:
  ```bash
  curl "http://worldtimeapi.org/api/timezone/America/New_York"
  ```
- This provides the most accurate timestamp in the required Eastern (New York) timezone

#### 4.1.2. Fallback Methods
1. **PowerShell Command**:
   ```powershell
   Invoke-WebRequest -Uri "https://worldtimeapi.org/api/timezone/America/New_York" | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty datetime
   ```
   - This command retrieves the exact time from worldtimeapi.org
   - Returns timestamp in Eastern (New York) timezone
   - Provides consistent format across all environments

2. **Manual Entry**: 
   - If automated methods fail, the AI will request the user to:
     * Visit worldtimeapi.org/timezone/America/New_York in a browser
     * Provide the current Eastern time manually
     * Format as YYYY-MM-DD HH:MM:SS [AM/PM]

---

### 4.2. Project Requirements

- **Related Sections**:
  - See Section 2.2 for requirements documentation
  - See Section 3.3 for quality assurance
  - See Section 5.2 for maintaining context

The following requirements were established in Requirements.md to ensure consistent timestamp handling across the project:

```markdown
## Timestamp Rules

### Source of Truth
- ALWAYS get the current time from: https://worldtimeapi.org/api/timezone/America/New_York
- NEVER use any other time source or make up timestamps

### Format Specification
- Format: [YYYY-MM-DD HH:MM:SS AM/PM]
- Example: [2024-12-22 04:26:34 PM]
- Components:
  - YYYY: Four-digit year
  - MM: Two-digit month (01-12)
  - DD: Two-digit day (01-31)
  - HH: Two-digit hour in 12-hour format (01-12)
  - MM: Two-digit minutes (00-59)
  - SS: Two-digit seconds (00-59)
  - AM/PM: Uppercase meridian indicator

### Usage Rules
- Use in ChangeLog.md for all entries
- Use in Tasks.md for section completion timestamps
- Always include the square brackets []
- Always use the exact format without variation
- Convert from 24-hour format to 12-hour format with am/pm

### Verification Steps
- Get current time from worldtimeapi.org
- Convert 24-hour time to 12-hour format
- Format with square brackets
- Include am/pm in uppercase
- Use exact spacing as shown in format
```

---

### 4.3. WorldTimeAPI Integration

- **Related Sections**:
  - See Section 5.1 for command execution
  - See Section 6.1 for API documentation
  - See Section 3.2 for best practices

WorldTimeAPI (worldtimeapi.org) is a free, open-source API that provides accurate, timezone-aware timestamps. It's particularly useful for:
- Getting consistent timestamps across different environments
- Handling timezone conversions automatically
- Ensuring accurate time recording in distributed systems

#### 4.3.1. Available Endpoints
- List all timezones: `http://worldtimeapi.org/api/timezone`
- Get specific timezone: `http://worldtimeapi.org/api/timezone/{area}/{location}`
- Get UTC time: `http://worldtimeapi.org/api/timezone/Etc/UTC`

#### 4.3.2. Customizing Your Timezone
To use a different timezone:

1. **Find Your Timezone**:
   ```powershell
   # List all available timezones
   Invoke-WebRequest -Uri "http://worldtimeapi.org/api/timezone" | Select-Object -ExpandProperty Content
   ```

2. **Common Timezone Examples**:
   - London: `/Europe/London`
   - Sydney: `/Australia/Sydney`
   - Tokyo: `/Asia/Tokyo`
   - Los Angeles: `/America/Los_Angeles`
   - Chicago: `/America/Chicago`

3. **Update Commands**:
   Replace `America/New_York` in the commands with your timezone:
   ```powershell
   # PowerShell example for London
   Invoke-WebRequest -Uri "https://worldtimeapi.org/api/timezone/Europe/London" | Select-Object -ExpandProperty Content | ConvertFrom-Json | Select-Object -ExpandProperty datetime
   ```

4. **Update Documentation**:
   - Ensure your chosen timezone is documented in the project
   - Update any timezone-dependent scripts or commands
   - Note timezone selection in ChangeLog.md

#### 4.3.3. Best Practices
- Always use consistent timezone across the project
- Document timezone selection in project configuration
- Consider team location when selecting timezone
- Account for daylight savings time handling

---

### 4.4. User Prompting and Reminders

- **Related Sections**:
  - See Section 5.3 for prompt generation
  - See Section 3.1 for process integration
  - See Section 7.3 for evaluation timing

The AI regularly prompts users for various actions to maintain project quality and consistency:

#### 4.4.1. Source Control Reminders
- **Periodic Saves**: Reminds users to commit changes to GitHub:
  - After completing a task
  - When significant progress is made
  - Before ending a development session
- **Commit Message Guidance**: Suggests structured commit messages that include:
  - Task reference number
  - Brief description of changes
  - Any special considerations

#### 4.4.2. Timestamp Requests
- Prompts for current timestamp when:
  - Creating new changelog entries
  - Updating task status
  - Documenting significant decisions
- Provides the exact command to run
- Explains how to format the timestamp correctly

#### 4.4.3. Other Common Prompts
- Running tests before commits
- Updating documentation
- Reviewing changes before implementation
- Verifying requirements alignment

---

## 5. AI Interaction Guidelines

This section provides comprehensive guidance for optimizing collaboration between users and the AI assistant. It covers communication best practices, session management, prompt generation, and troubleshooting strategies to ensure productive development sessions.

- **Related Sections**:
  - See Section 2.1 for Rules for AI guidelines
  - See Section 3.1 for development workflow
  - See Section 8.1 for collaboration benefits

---

### 5.1. Communication Best Practices

- **Related Sections**:
  - See Section 2.2 for requirements clarity
  - See Section 3.2 for process standards
  - See Section 7.1 for improvement feedback

#### 5.1.1. General Communication
- Use clear, concise language
- Provide specific examples when needed
- Ask clarifying questions when uncertain
- Maintain professional tone
- Focus on task-relevant details

#### 5.1.2. Command Execution Safety
- All commands require manual review before execution
- No automatic command execution is allowed
- This ensures:
  - Development process integrity
  - Validation of proposed changes
  - Optimization opportunities
  - Transparency in all operations

#### 5.1.3. Code Understanding
- Request explanations of complex code
- Collaborate on code reviews
- Discuss implementation alternatives
- Share knowledge about best practices
- Document important decisions

---

### 5.2. Session Management

- **Related Sections**:
  - See Section 3.1 for workflow integration
  - See Section 4.4 for user prompting
  - See Section 7.2 for session documentation

#### 5.2.1. Session Lifecycle
- **Starting a Session**:
  - Review previous work
  - Set clear objectives
  - Establish context
  - Define success criteria

- **During the Session**:
  - Track progress
  - Document decisions
  - Maintain focus
  - Address blockers

- **Ending a Session**:
  - Summarize accomplishments
  - Document next steps
  - Update task status
  - Record timestamps

#### 5.2.2. Project Knowledge
- Maintain awareness of:
  - Current project state
  - Recent changes
  - Pending tasks
  - Known issues
- Reference documentation regularly
- Track version changes

---

### 5.3. Prompt Generation

- **Related Sections**:
  - See Section 2.1 for guidance rules
  - See Section 3.2 for best practices
  - See Section 6.1 for documentation

#### 5.3.1. Effective Prompts
- Be specific and detailed
- Include relevant context
- Reference documentation
- Specify expected outcomes
- Provide examples when helpful

#### 5.3.2. Common Prompt Types
- Code explanation requests
- Implementation guidance
- Error resolution help
- Documentation updates
- Process clarification

---

### 5.4. Troubleshooting

- **Related Sections**:
  - See Section 3.3 for quality standards
  - See Section 6.2 for documentation help
  - See Section 7.1 for improvement process

#### 5.4.1. Common Pitfalls
- Unclear requirements
- Missing context
- Incomplete information
- Ambiguous requests
- Incorrect assumptions

#### 5.4.2. Resolution Strategies
- Review documentation
- Clarify requirements
- Provide more context
- Break down complex issues
- Test assumptions

#### 5.4.3. Error Resolution
- Clear error reporting
- Systematic debugging
- Solution validation
- Documentation updates
- Prevention strategies

---

### 5.5. Cursor IDE Features

- **Related Sections**:
  - See Section 3.1 for workflow integration
  - See Section 6.1 for feature documentation
  - See Section 8.2 for productivity benefits

#### 5.5.1. Code Navigation
- Quick file access
- Symbol search
- Reference finding
- Definition jumping
- Smart suggestions

#### 5.5.2. Refactoring Assistance
- Code restructuring
- Pattern implementation
- Style enforcement
- Quality improvements
- Performance optimization

#### 5.5.3. Integrated Development
- Version control
- Testing tools
- Documentation access
- Error detection
- Code completion

---

### 5.6. Testing Collaboration

- **Related Sections**:
  - See Section 3.3 for quality assurance
  - See Section 6.2 for test documentation
  - See Section 8.1 for quality benefits

#### 5.6.1. Test Development
- Test case design
- Coverage analysis
- Implementation guidance
- Quality validation
- Performance testing

#### 5.6.2. Test Review
- Code review integration
- Quality verification
- Documentation review
- Coverage assessment
- Improvement suggestions

---

## 6. Documentation Management

This section explores the diverse range of documentation resources available and how they are effectively utilized in development. It covers documentation sources, integration examples, usage patterns, and limitations to ensure comprehensive project documentation.

- **Related Sections**:
  - See Section 2.1 for Rules for AI documentation
  - See Section 3.1 for process documentation
  - See Section 8.1 for documentation benefits

---

### 6.1. Documentation Sources

- **Related Sections**:
  - See Section 2.2 for requirements docs
  - See Section 3.2 for best practices
  - See Section 5.2 for context management

#### 6.1.1. Core Documentation
- Requirements.md
- Tasks.md
- ChangeLog.md
- Rules for AI.md
- Project README

#### 6.1.2. Supporting Documentation
- Code comments and XML docs
- API documentation
- Test documentation
- Implementation guides
- Troubleshooting guides

---

### 6.2. Documentation Integration

- **Related Sections**:
  - See Section 3.1 for workflow integration
  - See Section 5.3 for documentation prompts
  - See Section 7.2 for evaluation docs

#### 6.2.1. Development Integration
- Inline documentation
- Code examples
- Implementation notes
- Decision records
- Version tracking

#### 6.2.2. Process Integration
- Task documentation
- Progress tracking
- Issue documentation
- Solution documentation
- Review documentation

---

### 6.3. Documentation Usage Patterns

- **Related Sections**:
  - See Section 3.2 for documentation standards
  - See Section 5.2 for session documentation
  - See Section 7.1 for improvement tracking

#### 6.3.1. Common Usage Patterns
- Reference lookup
- Implementation guidance
- Problem-solving
- Decision-making
- Knowledge sharing

#### 6.3.2. Documentation Maintenance
- Regular updates
- Version control
- Quality checks
- Consistency review
- Gap analysis

---

### 6.4. Documentation Limitations

- **Related Sections**:
  - See Section 3.3 for quality standards
  - See Section 5.4 for troubleshooting
  - See Section 7.3 for evaluation timing

#### 6.4.1. Known Limitations
- Update frequency
- Coverage gaps
- Version alignment
- Detail level
- Access control

#### 6.4.2. Mitigation Strategies
- Regular reviews
- Update processes
- Quality checks
- User feedback
- Continuous improvement

---

## 7. AI Self-Evaluation Process

This section explains how the AI's self-evaluation process contributes to continuous improvement and project success. It outlines the purpose, benefits, documentation format, and implementation process of regular self-evaluations.

- **Related Sections**:
  - See Section 2.1 for Rules for AI guidelines
  - See Section 3.1 for process integration
  - See Section 8.1 for quality benefits

---

### 7.1. Purpose and Benefits

- **Related Sections**:
  - See Section 2.2 for requirements alignment
  - See Section 3.3 for quality standards
  - See Section 5.1 for communication impact

#### 7.1.1. Continuous Improvement
- Identify areas for enhancement
- Track progress over time
- Adapt to changing needs
- Optimize performance
- Share best practices

#### 7.1.2. Knowledge Management
- Document lessons learned
- Build institutional knowledge
- Share successful strategies
- Prevent repeated issues
- Enhance collaboration

---

### 7.2. Self-Evaluation Documentation

- **Related Sections**:
  - See Section 2.4 for changelog integration
  - See Section 4.1 for timestamp usage
  - See Section 6.1 for documentation sources

#### 7.2.1. Documentation Format
- Clear section headers
- Specific examples
- Action items
- Success metrics
- Follow-up tasks

#### 7.2.2. Required Components
- Session timestamp
- Task references
- Progress assessment
- Challenges faced
- Solutions implemented
- Recommendations

---

### 7.3. Implementation Process

- **Related Sections**:
  - See Section 3.1 for workflow integration
  - See Section 5.2 for session management
  - See Section 6.2 for documentation practices

#### 7.3.1. Evaluation Timing
- End of major tasks
- Project milestones
- Regular intervals
- User-requested reviews
- Issue resolution

#### 7.3.2. User-Initiated Evaluations
- Request process
- Required information
- Response format
- Follow-up actions
- Documentation updates

---

### 7.4. Integration with Development

- **Related Sections**:
  - See Section 3.2 for best practices
  - See Section 5.4 for issue resolution
  - See Section 6.3 for documentation patterns

#### 7.4.1. Process Integration
- Development workflow
- Quality assurance
- Documentation updates
- Knowledge sharing
- Continuous improvement

#### 7.4.2. Feedback Implementation
- Action item tracking
- Progress monitoring
- Success measurement
- Process refinement
- Documentation updates

---

## 8. Benefits and Outcomes

This section outlines the comprehensive advantages of following a structured approach to AI-assisted development. It details both immediate and long-term benefits, focusing on sustainable development practices and continuous improvement.

- **Related Sections**:
  - See Section 2.1 for Rules for AI impact
  - See Section 3.1 for process benefits
  - See Section 7.1 for quality improvements

---

### 8.1. Immediate Benefits

- **Related Sections**:
  - See Section 2.2 for requirements alignment
  - See Section 5.1 for communication efficiency
  - See Section 6.1 for documentation value

#### 8.1.1. Development Efficiency
- Faster implementation
- Reduced errors
- Consistent quality
- Better organization
- Clear documentation

#### 8.1.2. Quality Improvements
- Standardized processes
- Thorough testing
- Comprehensive documentation
- Consistent formatting
- Error prevention

---

### 8.2. Project Management Benefits

- **Related Sections**:
  - See Section 3.1 for process integration
  - See Section 5.2 for session management
  - See Section 7.2 for progress tracking

#### 8.2.1. Task Management
- Clear organization
- Progress tracking
- Priority management
- Resource allocation
- Timeline adherence

#### 8.2.2. Documentation Benefits
- Comprehensive records
- Knowledge preservation
- Easy reference
- Clear communication
- Process improvement

---

### 8.3. Team Collaboration Benefits

- **Related Sections**:
  - See Section 3.2 for best practices
  - See Section 5.3 for communication
  - See Section 6.2 for documentation sharing

#### 8.3.1. Communication Improvements
- Clear expectations
- Consistent terminology
- Shared understanding
- Effective feedback
- Knowledge sharing

#### 8.3.2. Process Standardization
- Consistent workflows
- Quality standards
- Documentation practices
- Review processes
- Improvement cycles

---

### 8.4. Long-Term Advantages

- **Related Sections**:
  - See Section 2.1 for sustainable practices
  - See Section 7.1 for continuous improvement
  - See Section 6.3 for documentation evolution

#### 8.4.1. Sustainable Development
- Maintainable codebase
- Scalable processes
- Knowledge retention
- Quality assurance
- Continuous improvement

#### 8.4.2. Future Growth
- Adaptable framework
- Expandable processes
- Skill development
- Innovation support
- Team empowerment

---
