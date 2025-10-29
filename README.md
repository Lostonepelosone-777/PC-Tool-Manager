# 🖥️ PC Tool Manager

<div align="center">

![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)

**A comprehensive PC management and optimization suite with hardware monitoring, AI assistant, and system utilities.**

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Contributing](#-contributing) • [License](#-license)

</div>

---

## 🌟 Overview

PC Tool Manager is a modern, user-friendly desktop application built with Python and CustomTkinter. It provides a centralized interface for managing your PC's performance, monitoring hardware, optimizing resources, and more.

### Key Highlights

- 🔧 **Hardware Monitoring** - Real-time CPU, GPU, RAM, and temperature monitoring
- 🤖 **AI Assistant** - Integrated AI chat powered by Ollama
- 🧹 **Disk Cleanup** - Automated temporary file removal
- ⚡ **RAM Optimizer** - Memory optimization and process management
- 🛡️ **Security Sandbox** - Safe program execution environment
- 🌐 **Network Manager** - Connection testing and diagnostics
- 🎨 **Customizable UI** - Fully customizable themes and colors

---

## ✨ Features

### 🔧 Hardware Monitoring
- **Real-time Sensor Data**: Monitor CPU, GPU, and system temperatures
- **Fan Control**: Manage fan speeds and cooling profiles
- **External Tools Integration**: Seamless integration with HWiNFO64, CPU-Z, FanControl
- **Automatic Detection**: Auto-detects installed hardware monitoring tools
- **Dynamic Interface**: Buttons automatically update based on tool availability

### 🤖 AI Assistant
- **Integrated Chat**: Ask questions and get intelligent responses
- **Navigation Commands**: Natural language navigation to different sections
- **Ollama Support**: Local AI models for privacy-focused assistance
- **Model Management**: Download and manage multiple AI models

### 🧹 Disk & System Optimization
- **Temp File Cleanup**: Automatically locate and remove temporary files
- **RAM Optimization**: Intelligent memory management and process termination
- **Startup Manager**: Control which programs launch at startup
- **Task Manager Integration**: Quick access to system processes

### 🛡️ Security & Network
- **Sandbox Execution**: Run programs safely in isolated environments
- **VirusTotal Integration**: File scanning and security checks
- **Network Diagnostics**: Ping tests, speed tests, and connection analysis
- **Process Explorer**: Detailed system process information

### 🎨 Customization
- **Theme Support**: Light, dark, and custom themes
- **Color Customization**: Custom accent colors and UI elements
- **Font Management**: Adjustable font families and sizes
- **Real-time Preview**: See changes before applying

---

## 📦 Installation

### Prerequisites

- Windows 10/11
- Python 3.8 or higher
- pip (Python package manager)

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/Lost-777/pc-tool-manager.git
   cd pc-tool-manager
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the application**
   ```bash
   python main.py
   ```
   Or use the convenient launcher:
   ```bash
   python pc_tool_manager.pyw
   ```

---

## 🚀 Usage

### Starting the Application

#### Standard Launch
```bash
python main.py
```

#### Launch Without Console Window
```bash
python pc_tool_manager.pyw
```

#### Using Batch Files
Windows users can use the included batch files:
- `Avvia PC Tool Manager.bat` - Standard launch
- `start_with_cmd.vbs` - Launch without console

### Main Sections

#### 🏠 Home
Quick overview of system status and key metrics.

#### 🔧 Hardware Monitoring
- View real-time hardware statistics
- Monitor temperatures and fan speeds
- Launch external monitoring tools (HWiNFO64, CPU-Z)
- Control fans (requires external tools)

#### 🤖 AI Assistant
- Chat with AI using Ollama
- Natural language navigation
- Ask questions about your system
- Navigate to different sections using commands

#### 🧹 Disk Cleanup
- Scan for temporary files
- Clean browser cache
- Remove system temp files
- Free up disk space

#### ⚡ RAM Optimizer
- Monitor RAM usage in real-time
- Optimize memory
- End resource-heavy processes
- Quick access to Task Manager

#### 🛡️ Security Sandbox
- Run programs in isolated environment
- Scan files with VirusTotal
- Manage security tools
- Safe program execution

#### 🌐 Network Manager
- Test network connectivity
- Speed tests
- Ping diagnostics
- Connection information

#### ⚙️ Settings
- Customize theme and colors
- Adjust font settings
- Configure preferences

---

## 🔧 Configuration

### External Tools Setup

The application can automatically detect and integrate with these external tools:

1. **HWiNFO64** - Advanced hardware monitoring
2. **CPU-Z** - CPU and system information
3. **FanControl** - Fan speed control
4. **CrystalDiskInfo** - Disk health monitoring
5. **CrystalDiskMark** - Disk benchmarking

**Setup Methods:**
- Place tools in the `Tools/` folder
- Install normally in Program Files (auto-detected)
- Provide ZIP files (auto-extracted)
- Use shortcuts (.lnk files)

The application monitors the `Tools/` folder every 5 seconds and automatically updates the interface when tools are added or removed.

### AI Assistant Setup

To use the AI Assistant:

1. **Install Ollama**: https://ollama.com/download
2. **Download a model**: `ollama pull llama2`
3. **Start Ollama**: The app will auto-start Ollama if installed
4. **Start chatting**: Navigate to the AI Assistant section

---

## 📂 Project Structure

```
pc-tool-manager/
├── main.py                 # Main entry point
├── pc_tool_manager.pyw     # Launcher without console
├── gui.py                  # Main GUI application (CustomTkinter)
├── hardware_monitor.py     # Hardware monitoring module
├── requirements.txt        # Python dependencies
├── config.ini              # Application configuration
├── settings.ini            # User settings
├── Tools/                  # External tools directory
├── icon/                   # Application icons
└── README.md              # This file
```

---

## 🛠️ Development

### Requirements

- Python 3.8+
- All packages from `requirements.txt`

### Running from Source

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py

# Or run without console window
pythonw pc_tool_manager.pyw
```

### Key Dependencies

- `customtkinter` - Modern GUI framework
- `psutil` - System and process utilities
- `ollama` - AI/LLM integration
- `requests` - HTTP library
- `pywin32` - Windows-specific APIs
- `Pillow` - Image processing

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### How to Contribute

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Guidelines

- Follow PEP 8 Python style guide
- Add comments for complex logic
- Test thoroughly on Windows 10/11
- Update documentation if needed

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

### External Tools & Libraries

- **HWiNFO64** - Martin Malik - Hardware monitoring
- **CPU-Z** - CPUID - CPU information
- **FanControl** - Remi Mercier - Fan control
- **CrystalDiskInfo** - Crystal Dew World - Disk health
- **CrystalDiskMark** - Crystal Dew World - Disk benchmarking
- **CustomTkinter** - Tom Schimansky - Modern UI framework
- **Ollama** - AI/LLM platform

### Fonts & Icons

- Icons: Emoji and Unicode characters
- Fonts: System defaults with customizable options

---

## 📞 Support

- **Issues**: [GitHub Issues](https://github.com/Lost-777/pc-tool-manager/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Lost-777/pc-tool-manager/discussions)

---

## 🗺️ Roadmap

- [ ] Linux support
- [ ] macOS support
- [ ] Additional AI models
- [ ] Plugin system
- [ ] Cloud sync for settings
- [ ] Mobile companion app

---

<div align="center">

**Made with ❤️ by Lost-777**

⭐ Star this repo if you find it helpful!

</div>

