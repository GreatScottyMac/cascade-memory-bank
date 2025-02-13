# 🧠 Cascade Memory Bank

Enhance your Windsurf IDE experience with persistent project memory. Cascade Memory Bank enables the Cascade AI assistant to maintain deep project understanding across sessions, automatically documenting important context, decisions, and progress.

[View Developer's Guide](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/Developers/developer-primer.md) for detailed implementation information.

## 🚀 Quick Start

1. **Install**
   Download or copy the contents of these files:
   - [`.windsurfrules`](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/.windsurfrules) - Copy to your project root or paste into Windsurf's "Set Workspace AI Rules"
   - [`global_rules.md`](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/global_rules.md) - Copy to `~/.codeium/windsurf/memories/` or paste into Windsurf's Settings - Set Global AI Rules

2. **Configure Git**
   Important: If `memory-bank/` or `.windsurfrules` are gitignored, Cascade cannot see them. Use this recommended `.gitignore` setup for easy visibility toggling:

   ```bash
   # Ignore everything by default - delete this line temporarily when working with Cascade
   *

   # Version control list - always keep these lines
   !/.gitignore
   !/src/
   !/src/**
   !/package.json
   !/README.md
   !/docs/
   !/docs/**
   # Add more project files as needed
   ```

   **Usage:**
   - When working with Cascade: Delete the `*` line
   - Before committing: Add back the `*` line

   This approach provides a quick way to toggle Cascade's visibility while maintaining a clear list of version-controlled files.

   > **Note**: This repository version controls the memory bank files as it is the reference implementation.

3. **Start Using**
   - Begin by telling Cascade: "Follow the protocol in your .windsurfrules"
   - Memory bank initializes and loads all context
   - Project context updates automatically in real-time
   - Use "Update Memory Bank" or "UMB" trigger for manual updates (defined in `.windsurfrules`)

## 📁 Memory Bank Structure

The system maintains context through a `memory-bank/` directory containing four core files:

### Core Files

| File | Purpose | Updates |
|------|---------|---------|
| `activeContext.md` | Tracks session state and goals | Every session |
| `productContext.md` | Defines project scope and architecture | When scope changes |
| `progress.md` | Tracks work status and milestones | As tasks progress |
| `decisionLog.md` | Records important decisions | When decisions made |

## 🎯 Benefits

- **Enhanced Productivity**
  - No context loss between sessions
  - Reduced onboarding time for new tasks
  - Automatic documentation maintenance

- **Better Project Understanding**
  - Comprehensive decision history
  - Clear project evolution tracking
  - Maintained architectural context

- **Reduced Cognitive Load**
  - No manual note-taking needed
  - Important context always available
  - Natural conversation flow

## 📘 Usage Tips

- **Real-Time Updates**
  - Context updates happen automatically
  - Changes are logged immediately
  - Use "update memory bank" or "UMB" for manual updates if needed

- **Focus on Your Work**
  - Documentation happens automatically
  - Important context is preserved
  - Project history maintains itself

## 🔍 Need Help?

- [Read the Developer's Guide](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/Developers/developer-primer.md)
- Check the troubleshooting section
- Open an issue for support

## 📝 License

MIT License - See LICENSE file for details

## 🤝 Contributing

Contributions welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) first.

## ❤️ Support the Project

If you find Cascade Memory Bank valuable in your development workflow, consider [becoming a sponsor](https://github.com/sponsors/GreatScottyMac). Your support helps maintain and improve the project!
