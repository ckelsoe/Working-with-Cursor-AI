[← Previous: Development Process](./03_Development_Process.md) | [Next: AI Interaction →](./05_AI_Interaction.md)

# 4. Timestamp Management

This section explains how timestamps are generated and managed throughout the project lifecycle. It details the hierarchical approach to obtaining accurate timestamps, ensuring consistency across all documentation and logging.

**Related Sections**:
- See Section 2.3 for timestamp requirements
- See Section 2.4 for ChangeLog format
- See Section 7.2 for evaluation timing

---

## 4.1. Timestamp Generation and Retrieval

### 4.1.1. Primary Method
The primary method for obtaining timestamps is through the WorldTimeAPI:
```markdown
## Source of Truth
- ALWAYS get the current time from: https://worldtimeapi.org/api/timezone/America/New_York
- NEVER use any other time source or make up timestamps
```

### 4.1.2. Fallback Methods
When the primary method is unavailable:
1. Local system time with manual timezone adjustment
2. Previous valid timestamp with increment
3. User-provided timestamp with validation
4. Temporary placeholder with update flag

### 4.1.3. Timestamp Format
Standard format requirements:
```markdown
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
```

---

## 4.2. Project Requirements

### 4.2.1. Timestamp Usage
Required timestamp implementations:
```markdown
### Usage Rules
- Use in ChangeLog.md for all entries
- Use in Tasks.md for section completion timestamps
- Always include the square brackets []
- Always use the exact format without variation
- Convert from 24-hour format to 12-hour format with am/pm
```

### 4.2.2. Validation Rules
Each timestamp must:
- Be in correct timezone (ET)
- Follow ISO 8601 format
- Include timezone identifier
- Be chronologically valid
- Be properly formatted
- Be consistently applied

### 4.2.3. Error Handling
When timestamp issues occur:
- Log the error condition
- Use fallback methods
- Flag for review
- Document resolution
- Update if necessary
- Prevent duplicates

---

## 4.3. WorldTimeAPI Integration

### 4.3.1. API Implementation
Integration requirements:
- Proper error handling
- Response validation
- Format verification
- Timezone confirmation
- Cache management
- Fallback triggers

### 4.3.2. Response Handling
Processing steps:
- Validate response format
- Extract timestamp data
- Verify timezone
- Format conversion
- Error checking
- Cache updating

### 4.3.3. Timezone Management
1. **List Available Timezones**:
   ```powershell
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

---

## 4.4. User Prompting and Reminders

### 4.4.1. Source Control Reminders
- **Periodic Saves**: Reminds users to commit changes to GitHub:
  - After completing a task
  - When significant progress is made
  - Before ending a development session
- **Commit Message Guidance**: Suggests structured commit messages that include:
  - Task reference number
  - Brief description of changes
  - Any special considerations

### 4.4.2. Timestamp Requests
- Prompts for current timestamp when:
  - Creating new changelog entries
  - Updating task status
  - Documenting significant decisions
- Provides the exact command to run
- Explains how to format the timestamp correctly

### 4.4.3. Other Common Prompts
- Running tests before commits
- Updating documentation
- Reviewing changes before implementation
- Verifying requirements alignment

---

[← Previous: Development Process](./03_Development_Process.md) | [Next: AI Interaction →](./05_AI_Interaction.md) 