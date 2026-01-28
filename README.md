# Zaluno Agent

A lightweight agent that captures AI coding tool usage and sends analytics to [Zaluno](https://zaluno.com).

## Overview

Zaluno Agent runs in the background on your development machine, capturing usage data from AI coding assistants like Claude Code, Cursor, and others. It sends session analytics to Zaluno, giving engineering teams visibility into AI tool adoption and effectiveness.

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

Download the latest release from the [Releases](https://github.com/zaluno/agent/releases) page.

## Support

- Documentation: [docs.zaluno.com](https://docs.zaluno.com)
- Issues: [GitHub Issues](https://github.com/zaluno/agent/issues)
- Email: support@zaluno.com

## Data collection, usage, and retention

When you use Zaluno Agent, we collect AI conversation data from tools and apps installed on your computer, including Claude Code, Cursor, and others; and from our browser extension, if it's installed.

### How we use your data

See our [data usage policies](https://docs.zaluno.com/en/data-usage).

### Privacy safeguards

We have implemented several safeguards to protect your data, including limited retention periods for sensitive information, restricted access to user session data, and clear policies against using customer data for model training.

For full details, please review our [Terms of Service](https://zaluno.com/terms) and [Privacy Policy](https://zaluno.com/privacy).
