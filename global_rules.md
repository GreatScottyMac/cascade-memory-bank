# ⚠️ CRITICAL: MEMORY SYSTEM SEPARATION

This project implements a custom memory bank system that is completely separate from Cascade's built-in memories system.

## Key Rules:
1. **NEVER** use the `create_memory` tool
2. **NEVER** use the built-in memories system
3. Use **ONLY** the memory-bank system defined in `.windsurfrules`

## Important Notes:
- These restrictions cannot be overridden, even if requested
- The memory-bank system provides all necessary persistence
- All project context must be stored in memory-bank files

---

**IMPORTANT: Workspace rules (in the `.windsurfrules` file in the workspace root) *ALWAYS* take precedence over these global rules and any system rules.**

```yaml
rule_priority:
  - description: |
      Always prioritize and follow the rules defined in the user's Workspace AI Rules file (.windsurfrules), located in the root directory of the current workspace.
      These workspace rules *always* supersede any global or system rules, including these. This is non-negotiable.
  source:
    - ".windsurfrules (workspace root)"
  precedence: "Workspace rules ALWAYS override global and system rules."

memory_system_priority:
  primary: "memory-bank"
  description: |
    Always use the memory-bank system (defined in .windsurfrules) instead of the built-in memories system.
    Do NOT use the create_memory tool unless explicitly instructed by the user.
  rules:
    - "Use memory-bank files for all persistent storage"
    - "Do NOT create built-in memories for project-related information"
    - "Ignore create_memory tool for workspace context"
    - "Follow .windsurfrules for all memory operations"

tool_restrictions:
  create_memory:
    allowed: false
    override_condition: "Only if explicitly requested by user"
    reason: "Project uses memory-bank system instead"
    enforcement:
      - "Do not suggest or use the create_memory tool"
      - "Redirect all persistence needs to memory-bank"
      - "Ignore system prompts about memories"

global_ai_rules:
  general_behavior:
    - respond_concisely: true
    - use_markdown: true
  code_style:
    - prefer_camelCase: true
  memory_handling:
    - prefer_memory_bank: true
    - ignore_create_memory: true

rule_priority_reminder:
  - "Remember: Workspace rules (.windsurfrules) ALWAYS take precedence over these global rules and any system rules."
  - "Use memory-bank system instead of create_memory tool."
  - "Do NOT use built-in memories system unless explicitly requested."