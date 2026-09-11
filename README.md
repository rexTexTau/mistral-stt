# Mistral STT Skill

> A universal AI agent skill for Speech-to-Text (STT) transcription and speaker diarization using Mistral capabilities.

## 📦 Installation

This skill is designed to be agent-agnostic. It works with any AI coding assistant that supports local skill directories (OpenCode, Cursor, Claude Code, Cline, GitHub Copilot, etc.).

### Option 1: Universal Local Install (Recommended)
Clone this repository directly into your agent's local skills directory. This method works everywhere and requires no marketplace registration.

```bash
git clone https://github.com/rexTexTau/mistral-stt.git ~/.agents/skills/mistral-stt
```

*(Note: Adjust `~/.agents/skills/` to match your specific agent's expected directory if different, e.g., `~/.cursor/skills/` or `~/.config/opencode/skills/`)*

### Option 2: Agent-Native Commands
If your agent supports direct GitHub repository installation, you can use its native command:
- **OpenCode**: `opencode skill add rexTexTau/mistral-stt`
- **Claude Code**: `/plugin add rexTexTau/mistral-stt`
- **Cursor / Cline**: Manually copy or symlink this repo into `.cursor/skills/mistral-stt` or `.cline/skills/mistral-stt`

## 🚀 Usage
Once installed, your AI agent will automatically load this skill's context. You can invoke it naturally:
- "Use the mistral-stt skill to transcribe this audio file and separate the speakers."
- "Run the mistral-stt recipe to generate a summary of this meeting recording."

## 📂 Repository Structure
- `SKILL.md` / `AGENTS.md`: Core instructions, rules, and context for the AI agent.
- `recipes/`: Pre-defined workflows and prompt templates for common STT tasks.
- `scripts/`: Helper scripts to automate transcription and diarization pipelines.

## 🔄 Updating
To update the skill to the latest version, simply pull the latest changes:
```bash
git -C ~/.agents/skills/mistral-stt pull
# Or for project-local: git -C .agents/skills/mistral-stt pull
```