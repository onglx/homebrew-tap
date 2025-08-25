# OnglX Deploy - Homebrew Tap

Official Homebrew tap for OnglX Deploy CLI.

## 🍺 Installation

```bash
# Add the tap
brew tap onglx/tap

# Install OnglX Deploy
brew install onglx-deploy

# Verify installation
onglx-deploy --version
```

## 🔄 Updates

```bash
# Update the tap
brew update

# Upgrade to latest version
brew upgrade onglx-deploy
```

## 🚀 Quick Start

```bash
# Initialize a new project
onglx-deploy init

# Deploy your API
onglx-deploy deploy

# Check deployment status  
onglx-deploy status
```

## 🌟 What is OnglX Deploy?

OnglX Deploy is a CLI tool that deploys AI APIs to AWS in 30 seconds with 85% cost savings.

### Key Features
- **⚡ 30-second deployments** - From code to production API
- **💰 85% cost reduction** - Optimized AWS infrastructure
- **🤖 AI-optimized** - Built for inference workloads
- **📊 Auto-scaling** - Handle traffic spikes automatically
- **🌍 Global CDN** - Low-latency worldwide
- **🔒 Enterprise-ready** - VPC, IAM, logging, monitoring

### Supported Platforms
- **macOS**: Intel (x64) and Apple Silicon (arm64)
- **Linux**: x64 and arm64
- **Windows**: Use npm or direct download

## 📋 Requirements

- **Homebrew** (macOS/Linux)
- **AWS Account** with CLI configured
- **Python 3.9+** (for inference APIs)
- **Git** (optional, for advanced features)

## 💻 Alternative Installation

### npm (All Platforms)
```bash
npm install -g @onglx/deploy-cli
```

### Direct Download
Download from [releases](https://github.com/onglx/homebrew-tap/releases).

## 🆘 Troubleshooting

### Tap Issues
```bash
# Remove and re-add tap
brew untap onglx/tap
brew tap onglx/tap

# Force reinstall
brew uninstall onglx-deploy
brew install onglx-deploy
```

### macOS Security
If macOS blocks the binary:
```bash
# Allow the binary (one-time)
sudo xattr -rd com.apple.quarantine $(which onglx-deploy)
```

### Common Issues
- **"Command not found"**: Make sure `/opt/homebrew/bin` (Apple Silicon) or `/usr/local/bin` (Intel) is in your PATH
- **"Permission denied"**: Run `brew doctor` to fix Homebrew permissions
- **"Checksum mismatch"**: Clear Homebrew cache with `brew cleanup --prune=all`

## 📚 Documentation

- **Full Documentation**: https://docs.onglx.com
- **Examples**: https://github.com/onglx/examples
- **API Reference**: https://docs.onglx.com/api

## 🐛 Bug Reports & Support

- **Issues**: https://github.com/onglx/deploy/issues
- **Email**: support@onglx.com
- **Discord**: https://discord.gg/onglx

## 🔧 For Maintainers

### Release Process
This tap is automatically updated by the private source repository when new versions are released.

### Manual Formula Update
```bash
# Update version and URLs in Formula/onglx-deploy.rb
brew audit --new-formula Formula/onglx-deploy.rb
brew test-bot --only-setup
```

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

---

**Made with ❤️ by the OnglX team**