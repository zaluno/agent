# Zaluno Agent

A lightweight agent that captures AI coding tool usage and sends analytics to [Zaluno](https://zaluno.com).

## Overview

Zaluno Agent runs in the background on your development machine, capturing usage data from AI coding assistants like Claude Code, Cursor, and others. It sends anonymized analytics to Zaluno, giving engineering teams visibility into AI tool adoption and effectiveness.

## Installation

### macOS

Download the latest release from the [Releases](https://github.com/zaluno/agent/releases) page.

```bash
# Install via Homebrew (coming soon)
brew install zaluno/tap/agent
```

### Linux

```bash
# Download and install
curl -fsSL https://github.com/zaluno/agent/releases/latest/download/zaluno-agent-linux-amd64 -o zaluno-agent
chmod +x zaluno-agent
sudo mv zaluno-agent /usr/local/bin/
```

### Windows

Download the latest `.exe` from the [Releases](https://github.com/zaluno/agent/releases) page.

## Usage

1. Sign in to your Zaluno account at [zaluno.com](https://zaluno.com)
2. Navigate to Settings > Devices and generate a device token
3. Run the agent with your token:

```bash
zaluno-agent --token YOUR_DEVICE_TOKEN
```

The agent will run in the background and automatically capture AI tool usage.

## Privacy

Zaluno Agent is designed with privacy in mind:

- Raw conversation transcripts are processed locally
- Only aggregated insights and metadata are sent to Zaluno servers
- No code snippets or sensitive content leaves your machine
- You control what data is captured and shared

See our [Privacy Policy](https://zaluno.com/privacy) for more details.

## Configuration

Configuration file location:
- macOS: `~/.config/zaluno/agent.toml`
- Linux: `~/.config/zaluno/agent.toml`
- Windows: `%APPDATA%\zaluno\agent.toml`

Example configuration:

```toml
[agent]
token = "your-device-token"
log_level = "info"

[capture]
enabled_tools = ["claude-code", "cursor", "chatgpt"]
```

## Support

- Documentation: [docs.zaluno.com](https://docs.zaluno.com)
- Issues: [GitHub Issues](https://github.com/zaluno/agent/issues)
- Email: support@zaluno.com

## License

MIT License - see [LICENSE](LICENSE) for details.
