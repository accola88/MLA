# My Local Assistant (MLA)

**Your private AI assistant for Windows — 100% local, 100% offline. Free to use.**

My Local Assistant runs powerful AI models directly on your own computer. No cloud, no account, no subscription — your documents, dictations and conversations never leave your device.

![Chat](screenshots/chat.png)

## Features

- 💬 **Chat with tools** — ask questions, summarize files, search your folders. The assistant can read documents (PDF, Word, Excel), search the web (optional) and tells you which sources it used.
- 📅 **Scheduled tasks** — automatic daily briefings (e.g. news research) created at your chosen time via templates and skills.
- 🎙️ **Dictation everywhere in Windows** — global hotkey opens a small dictation window on top of any program; speech recognition (Whisper) runs locally.
- 🕵️ **Document anonymization** — pseudonymize or redact personal data in documents before sharing them (detection optimized for German documents). Includes PDF → Markdown conversion, even for scanned files.
- 📚 **Knowledge chat** — connect your Obsidian vault or SiYuan notes and ask questions about your own knowledge.
- ⚡ **GPU acceleration (optional)** — one switch, a safe self-test, and the model is distributed automatically across GPU memory and RAM (Vulkan, works with NVIDIA/AMD/Intel).
- 🌍 **5 languages** — the entire interface and the assistant's replies are available in **English, German (Deutsch), French (Français), Spanish (Español) and Russian (Русский)** — switchable live in the settings.
- 🔌 **Internet kill switch** — one click disables every online feature; a status indicator always shows whether you are online or 100% local.
- 🔄 **Built-in updates** — the app checks for new versions on GitHub (only when online, download only on your click) and shows a "What's new" summary after updating.

## Screenshots

| Settings | Models & system check |
|---|---|
| ![Settings](screenshots/settings.png) | ![Models](screenshots/models.png) |

| Document processing | What's new |
|---|---|
| ![Processing](screenshots/processing.png) | ![What's new](screenshots/whats-new.png) |

## Download & installation

1. Download the latest `My Local Assistant_x64-setup.exe` from the [Releases page](https://github.com/accola88/MLA/releases/latest).
2. Run the installer. Windows SmartScreen may show a warning because the app is not commercially code-signed — click **"More info" → "Run anyway"**.
3. On first start, a short setup guides you through name, AI model download and folder selection.

**Requirements:** Windows 10/11 (64-bit), 8 GB RAM minimum (16 GB recommended), ~10 GB free disk space for the app and one AI model.

## Privacy

Everything — AI models, speech recognition, your documents and notes — is processed locally on your machine. Internet access is used only for optional features (web search, model downloads, update check) and can be disabled completely with the built-in kill switch.

## License

© accola88. All rights reserved.

**Free to use** for personal purposes. Redistribution or modification requires permission. This application bundles open-source components — see `THIRD-PARTY-NOTICES.txt` included with the installation.
