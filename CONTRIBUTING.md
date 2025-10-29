# Contributing to PC Tool Manager

Thank you for your interest in contributing to PC Tool Manager! This document provides guidelines and instructions for contributing to the project.

## 🤝 How to Contribute

### Reporting Bugs

If you find a bug, please create an issue with:

1. **Clear description** of the problem
2. **Steps to reproduce** the bug
3. **Expected behavior** vs actual behavior
4. **Screenshots** if applicable
5. **System information** (OS version, Python version)

### Suggesting Features

Feature suggestions are welcome! Please include:

1. **Use case** - Why is this feature useful?
2. **Proposed solution** - How should it work?
3. **Alternatives considered** - Other approaches you've thought about

### Code Contributions

#### Getting Started

1. Fork the repository
2. Clone your fork
3. Create a new branch for your feature
4. Make your changes
5. Test thoroughly
6. Submit a pull request

#### Development Setup

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/pc-tool-manager.git
cd pc-tool-manager

# Install dependencies
pip install -r requirements.txt

# Create a feature branch
git checkout -b feature/your-feature-name
```

#### Coding Standards

- **Python Style**: Follow PEP 8
- **Naming**: Use descriptive variable and function names
- **Comments**: Add comments for complex logic
- **Docstrings**: Document functions and classes
- **Testing**: Test your changes before submitting

#### Commit Messages

Use clear, descriptive commit messages:

```
feat: Add dark mode support
fix: Resolve memory leak in hardware monitor
docs: Update installation instructions
refactor: Improve code organization
```

#### Pull Request Process

1. **Update documentation** if your changes affect user-facing features
2. **Add tests** if applicable (though currently we don't have formal tests)
3. **Test on Windows 10/11** to ensure compatibility
4. **Update the README** if needed
5. **Link related issues** in your PR description

### Development Guidelines

#### GUI Development

- Use CustomTkinter for all UI components
- Follow the existing design patterns
- Maintain responsiveness during operations
- Provide visual feedback for long-running operations

#### Hardware Monitoring

- Use the existing `hardware_monitor.py` module as reference
- Handle errors gracefully
- Support both admin and non-admin modes
- Don't block the UI thread

#### AI Assistant

- Support multiple AI models
- Handle connection errors gracefully
- Provide helpful navigation commands
- Maintain conversation history

### Code Structure

Key modules:

- `gui.py` - Main application and UI
- `hardware_monitor.py` - Hardware monitoring logic
- `main.py` - Application entry point
- `pc_tool_manager.pyw` - Launcher script

### Testing

While we don't have formal unit tests yet, please:

1. **Manual test** your changes thoroughly
2. **Test edge cases** and error conditions
3. **Verify UI responsiveness**
4. **Check for memory leaks** in long-running operations

### Documentation

When adding features:

1. Update the README if it's a user-facing feature
2. Add inline comments for complex logic
3. Update this file if contributing guidelines change
4. Document new dependencies in `requirements.txt`

## 🎯 Feature Priorities

Current priorities:

1. **Bug fixes** - Always welcome
2. **Performance improvements** - Optimize existing features
3. **UI/UX enhancements** - Improve user experience
4. **Platform support** - Linux, macOS support
5. **New monitoring features** - Additional hardware sensors

## 💬 Communication

- **GitHub Issues**: For bug reports and feature requests
- **GitHub Discussions**: For questions and general discussion
- **Pull Requests**: For code contributions

## 📜 Code of Conduct

Be respectful, constructive, and collaborative. We're all here to make this project better!

---

Thank you for contributing to PC Tool Manager! 🎉

