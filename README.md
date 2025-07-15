# ByteAgent Flatpak

This repository contains the Flatpak manifest for ByteAgent, an AI Desktop Assistant with 64+ Professional Tools.

## About ByteAgent

ByteAgent is an AI-powered development assistant that provides 64+ professional tools for system monitoring, network analysis, security testing, and file operations. Perfect for developers, system administrators, and IT professionals.

## Installation

### From Flathub (Recommended)

```bash
flatpak install flathub com.byteagent.ByteAgent
```

### From this repository

```bash
git clone https://github.com/aldrin-ai/byteagent-flatpak.git
cd byteagent-flatpak
flatpak-builder --user --install --force-clean build-dir com.byteagent.ByteAgent.yml
```

## Running

```bash
flatpak run com.byteagent.ByteAgent
```

## Features

- 64+ cross-platform professional tools
- AI-powered command execution
- Network diagnostics and security testing
- File operations and system monitoring
- Power consumption analysis
- Web analysis and performance testing

## Links

- [Main Repository](https://github.com/aldrin-ai/byte-agent)
- [Homepage](https://github.com/aldrin-ai/byte-agent)
- [Bug Reports](https://github.com/aldrin-ai/byte-agent/issues)

## License

This Flatpak manifest is provided under the MIT License.
The ByteAgent application itself is licensed under its own terms.