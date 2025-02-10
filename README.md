# 🧠 Cascade Memory Bank

Enhance your Windsurf IDE experience with persistent project memory. Cascade Memory Bank enables the Cascade AI assistant to maintain deep project understanding across sessions, automatically documenting important context, decisions, and progress.

[View Developer's Guide](developer-primer.md) for detailed implementation information.

## 🚀 Quick Start

1. **Install**
   ```bash
   git clone https://github.com/GreatScottyMac/cascade-memory-bank.git
   cp cascade-memory-bank/.windsurfrules /path/to/your/project/
   ```
   Or paste `.windsurfrules` contents into Windsurf's "Set Workspace AI Rules".

2. **Start Using**
   - Begin any conversation with Cascade
   - Memory bank initializes automatically
   - Project context builds naturally through your interactions

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

- **Just Chat Naturally**
  - No special commands needed
  - Context builds automatically
  - Updates happen in real-time

- **Focus on Your Work**
  - Documentation happens automatically
  - Important context is preserved
  - Project history maintains itself

## 🔍 Need Help?

- [Read the Developer's Guide](developer-primer.md)
- Check the troubleshooting section
- Open an issue for support

## 📝 License

MIT License - See LICENSE file for details

## 🤝 Contributing

Contributions welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) first.

## ❤️ Support the Project

If you find Cascade Memory Bank valuable in your development workflow, consider [becoming a sponsor](https://github.com/sponsors/GreatScottyMac). Your support helps maintain and improve the project!
