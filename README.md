# 🧠 Cascade Memory Bank

Enhance your Windsurf IDE experience with persistent project memory. Cascade Memory Bank enables the Cascade AI assistant to maintain deep project understanding across sessions, automatically documenting important context, decisions, and progress.

[View Developer's Guide](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/Developers/developer-primer.md) for detailed implementation information.

## 🚀 Quick Start

### Install
#### 1. Download or copy the contents of these files:
* [`.windsurfrules`](https://github.com/GreatScottyMac/cascade-memory-bank/blob/main/.windsurfrules) - Copy to your project root or paste into "Add workspace rules"
* Optionally: Paste into "Add global rules"

    <img src="https://raw.githubusercontent.com/GreatScottyMac/cascade-memory-bank/main/cascade-memories-ui.png" alt="Prompt Settings Icon" width="300"/>

<br>

#### 2. Turn off "Auto-Generate Memories": [Ctrl + ,] - Configuration - Auto-Generate Memories

   <img src="https://raw.githubusercontent.com/GreatScottyMac/cascade-memory-bank/main/auto-generate_memories_off.png" alt="Prompt Settings Icon" width="300"/>

<br>

### Start Using
   - Begin by telling Cascade: "Follow the protocol in your rules" (you may also include the initial task)
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