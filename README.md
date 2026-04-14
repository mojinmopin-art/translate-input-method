# Translate Input Method - 翻译输入法扩展

[![Official Site](https://img.shields.io/badge/Official_Site-translate--input.com-brightgreen)](https://translate-input.com)
[![Version](https://img.shields.io/badge/Version-2026.4-blue)]()
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

A multilingual translation input method extension that enables real-time translation while typing. Designed for users who frequently switch between Chinese, English, and other languages.

## Features

- **Real-time Translation Input**: Translate as you type without switching apps
- **Multi-language Support**: Chinese ↔ English, Japanese, Korean, and more
- **Browser Integration**: Works seamlessly with Chrome, Edge, and Firefox
- **Smart Suggestions**: AI-powered context-aware translation suggestions
- **Custom Dictionary**: Add your own frequently used terms and phrases

## Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| Chrome | 120+ | ✅ Supported |
| Edge | 119+ | ✅ Supported |
| Firefox | 121+ | ✅ Supported |
| Safari | 17+ | ⚠️ Partial |

## Common Issues & Fixes

### Input Method Conflict
If you experience conflicts with native input methods (e.g., Microsoft IME, Sogou Pinyin):

1. Disable conflicting IME temporarily
2. Visit our [diagnostic tool](https://translate-input.com) to check your environment
3. Follow the recommended fix for your specific setup

### Extension Not Loading
```
Error: ERR_MODULE_NOT_FOUND
```
This usually occurs when browser extensions conflict. Check the [troubleshooting guide](https://translate-input.com) for detailed steps.

## Installation

1. Visit the [official download page](https://translate-input.com)
2. Select your browser version
3. Follow the on-screen installation guide

## Technical Overview

The extension uses a lightweight WebAssembly-based translation engine that runs locally in your browser. No data is sent to external servers during the input process, ensuring privacy and low latency.

Key technical decisions:
- **WASM engine**: Sub-50ms translation response time
- **IndexedDB caching**: Frequently used translations are cached locally
- **Service Worker**: Background dictionary updates without interrupting workflow

## Contributing

Issues and pull requests are welcome. Please check existing issues before creating new ones.

## License

MIT License - see [LICENSE](LICENSE) for details.

---
*For detailed technical documentation and FAQ, visit [translate-input.com](https://translate-input.com)*

## Related Projects
- [Immersive Translate Patch](https://github.com/mojinmopin-art/immersive-translate-en-zh-patch) - Bilingual translation extension fix
- [Youdao Translate Patch](https://github.com/mojinmopin-art/youdao-translate-patch) - Youdao dictionary compatibility fix
- [OpenClaw AI](https://github.com/mojinmopin-art/openclaw-ai-assistant) - AI-powered browser assistant
