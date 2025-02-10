# 🧠 Cascade Memory Bank

A persistent memory system for Cascade, the agentic AI assistant in Windsurf IDE. Maintains deep project understanding across sessions through structured documentation and context tracking.

## 🚀 Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/GreatScottyMac/cascade-memory-bank.git
   ```

2. Copy the `.windsurfrules` file to your project root
   ```bash
   cp cascade-memory-bank/.windsurfrules /path/to/your/project/
   ```

   Or copy its contents and paste into "Set Workspace AI Rules" in Windsurf settings.

## 📁 Memory Bank Structure

The system maintains context through a `memory-bank/` directory containing four core files:

### Core Files

| File | Purpose | Updates |
|------|---------|---------|
| `activeContext.md` | Tracks session state and goals | Every session |
| `productContext.md` | Defines project scope and architecture | When scope changes |
| `progress.md` | Tracks work status and milestones | As tasks progress |
| `decisionLog.md` | Records important decisions | When decisions made |

## 🔄 How It Works

1. **Initialization**
   - On first interaction, Cascade creates the `memory-bank/` directory
   - Generates core files with initial structure
   - Establishes baseline project context

2. **During Sessions**
   - Automatically reads and processes all Memory Bank files
   - Updates context based on interactions
   - Tracks progress and decisions
   - Maintains cross-references between files

3. **Between Sessions**
   - Preserves knowledge across sessions
   - Maintains consistent project understanding
   - Provides continuity in development

## 🛠️ Best Practices

1. **Let Cascade Manage the Memory Bank**
   - Files are automatically created and updated
   - Structure is maintained consistently
   - Cross-references are handled automatically

2. **Regular Interactions**
   - Start sessions with simple greetings
   - Allow context building before complex tasks
   - Review progress at session end

## ⚠️ Troubleshooting

If Cascade seems to lack context:
1. Verify `memory-bank/` directory exists
2. Check core files are present
3. Ensure file permissions are correct
4. Start a new session to rebuild context

## 📝 License

MIT License - See LICENSE file for details

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
