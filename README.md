# Hermes Mobile Client

**Mobile client for Hermes Agent** — Run a full AI coding agent directly on your phone.

Built by **Nous Research**, Hermes brings the power of an autonomous AI agent to your mobile device. Install a complete Ubuntu environment in Termux and control your agent right from your phone.

## Features

✨ **Full Ubuntu Environment** on Android via Termux
- Complete Linux environment with all development tools
- No desktop needed — everything runs on your phone

🤖 **Hermes Agent Gateway**
- Full-featured AI coding agent
- Real-time command execution
- Code generation and debugging

🔄 **9Router Integration**
- Built-in proxy and routing capabilities
- Direct API access from the app

📱 **Mobile-First Interface**
- Beautiful Flutter + React Native UI
- Real-time output and error handling
- Chat-based interaction

🚀 **Local Execution**
- Everything runs on your device
- Privacy-first design
- No cloud dependencies

## System Requirements

- **Device:** Android phone with ARM64 processor
- **RAM:** Minimum 4GB (8GB recommended)
- **Storage:** 5GB+ free space
- **OS:** Android 10+

### Tested On
- POCO X6 Pro (2311DRK48G)
- Other ARM64 Android devices

## Installation

### 1. Install Termux
Download Termux from [F-Droid](https://f-droid.org/packages/com.termux/) (recommended) or [Google Play](https://play.google.com/store/apps/details?id=com.termux).

### 2. Install Hermes Mobile Client APK
- Download `app-release.apk` from [Releases](https://github.com/PARHAM403/Hermes-Mobile-Client/releases)
- Transfer to your phone
- Install using your file manager or:
  ```bash
  adb install app-release.apk
  ```

### 3. Launch and Set Up
Open Hermes Mobile Client from your app drawer and follow the in-app setup guide.

## Quick Start

1. **Install Ubuntu Environment** (one-time, ~5min)
   - Tap "Install" in the app
   - Wait for proot-distro to download Ubuntu

2. **Set Up Bridge**
   - Generate or provide a secure key (16+ chars)
   - Connect from the Control tab

3. **Run Commands**
   - Use the chat interface to interact with your agent
   - Commands execute in real-time with visible output

## Architecture

```
Hermes Mobile Client (Flutter/React Native)
         ↓
   Hermes Agent Gateway
   (Local on Ubuntu)
         ↓
      9Router
   (Proxy/API)
         ↓
   Development Tools
   (Python, Node, Git, etc.)
```

## Usage Examples

```bash
# Inside Hermes chat interface

/help              # Show available commands
/gateway           # Check gateway status
/models            # List available AI models
/set-home          # Set current chat as home

# Run code
python my_script.py
npm install
git clone <repo>
```

## Configuration

### Model Selection
Change AI model from the Models tab:
- Claude Sonnet
- GPT-4
- Gemini
- Local LLMs (Ollama)

### Gateway Settings
Available from Help → Settings:
- API Server address
- Port configuration (default: 8642)
- Approval modes (manual/smart)

## Troubleshooting

### Bridge Connection Issues
- Ensure port 8642 is accessible
- Check Ubuntu environment installation status
- Restart gateway from Control tab

### Performance
- Close other apps to free RAM
- For heavy tasks, consider external power

### Storage Full
- Check Ubuntu size: `df -h`
- Clean package cache: `apt clean`

## File Structure

```
Hermes-Mobile-Client/
├── README.md               # This file
├── LICENSE                 # License information
├── app-release.apk         # Installable APK
└── docs/                   # Documentation
    ├── SETUP.md           # Detailed setup guide
    ├── COMMANDS.md        # Available commands
    └── TROUBLESHOOTING.md # Common issues
```

## Contributing

This is the official mobile client for Hermes Agent. For feature requests or bug reports:

1. Check existing [Issues](https://github.com/PARHAM403/Hermes-Mobile-Client/issues)
2. Create a new Issue with details
3. Submit Pull Requests for improvements

## License

Hermes Agent is built by **Nous Research**. See LICENSE file for terms.

## Community

- 💬 **Telegram:** Join our community
- 🐛 **Issues:** Report bugs
- 💡 **Discussions:** Share ideas

## Resources

- [Hermes Agent Documentation](https://hermes-agent.nousresearch.com/)
- [Termux Wiki](https://wiki.termux.com/)
- [proot-distro](https://github.com/termux/proot-distro)

---

**Made by:** Nous Research
**Maintained by:** Community
**Last Updated:** October 2026

For support and updates, visit: [Hermes Agent](https://hermes-agent.nousresearch.com/)
