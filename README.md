# My Local Assistant (MLA)

**Your private AI assistant — 100% local, 100% offline. Free to use.**
**Available for Windows and Linux.**

My Local Assistant runs powerful AI models directly on your own computer. No cloud, no account, no subscription — your documents, dictations and conversations never leave your device.

![Chat](chat.jpg)

## Why MLA?

- 🧠 **Fully automatic memory management** — models load on demand and unload by themselves after idle time (within ~2 minutes in tray mode). In standby the whole backend needs under 50 MB of RAM; heavy jobs run in throwaway worker processes that return 100% of their memory when done. You never manage anything manually.
- 🔒 **Radically private** — everything (AI models, speech recognition, your documents, notes and dictations) is processed on your machine. One click on the built-in **internet kill switch** disables every online feature; a status indicator always shows whether you are online or 100% local.
- 🌍 **5 languages, switchable live** — the entire interface and the assistant's replies in **English, Deutsch, Français, Español, Русский**. Choosing a language also adapts dictation and keyboard-shortcut handling.

## Features

### 🕵️ Document anonymization — MLA's specialty
Remove personal data from documents before sharing them: **pseudonymize** (readable markers like `«PERSON-1»`, `«FIRMA-2»` — the same person keeps the same marker through the whole text) or **redact** (████). Detection is optimized for German documents and combines pattern recognition, NLP and your own **always/never word lists** (company names, projects, technical terms), plus an optional second pass by the language model for anything that slipped through. Works on pasted text or whole files (PDF, Word, Excel).

![Processing](processing.jpg)

### 📄 PDF → Markdown conversion
Turn PDFs — **including scanned ones** (built-in OCR pipeline) — into clean, structured Markdown with headings and tables. Great for feeding documents into note apps, wikis or further AI processing. The required Java component ships with the app; nothing to install.

### 💬 Chat with tools
Ask questions, summarize files, search your folders. The assistant can read documents (PDF, Word, Excel), search the web (optional), look things up in your saved briefings and dictations — and always tells you which sources it used. Attach a file via the **+** button and just say what to do with it. Anything that writes to disk asks for your confirmation first.

### 🎙️ Dictation & voice assistant
A global hotkey (default `Ctrl+Alt+Space`) opens a small always-on-top dictation window over any program. Speak, get live text (local Whisper), copy it anywhere — **or ask the AI directly from the mini window** and get an answer without ever opening the main app. Dictations are saved automatically and can sync to Obsidian/SiYuan as notes.

### 📅 Scheduled & recurring tasks
Create jobs that run automatically — daily, on weekdays, weekly or hourly — built from reusable skills and templates (e.g. "research today's news on topic X and write a briefing"). Integrates with the **Windows Task Scheduler**; results are saved as plain Markdown files you can open with any program.

### 🤖 Models: always current — or bring your own
A curated catalog of recommended **GGUF models** (Qwen, Gemma, …) that stays up to date through the app's update mechanism, **without** needing a new app version. Or import **your own models** straight from Hugging Face: LLMs as `.gguf` files, speech recognition as faster-whisper repos. A built-in **system check** rates every model for *your* hardware — including whether it fits into your GPU memory — and a **benchmark** measures real tokens-per-second on your machine.

### ⚡ Optional GPU acceleration
One switch in the settings: the app safely **tests itself first** (in a separate process — a driver problem can never take down the app) and then distributes the model automatically across GPU memory and RAM, based on your actual VRAM. Vulkan-based, works with NVIDIA, AMD and Intel. CPU stays the default; the system check tells you honestly whether GPU mode is worth it on your hardware — or why it is not available (e.g. missing Vulkan driver).

### 📚 Knowledge chat
Connect your **Obsidian** vault or **SiYuan** notes, build a local search index, then ask "What do my notes say about project X?". Tell the assistant "remember this…" and it stores facts in its local knowledge — after your confirmation.

### 🔄 Built-in updates
The app checks GitHub for new versions (only when online, notification can be turned off, download only on your click) and shows a **"What's new"** summary after updating.

![What's new](whats-new.jpg)

## More screenshots

![Settings](settings.jpg)

![Help](help.jpg)

## Download & installation

All downloads: **[Releases page](https://github.com/accola88/MLA/releases/latest)**

### 🪟 Windows

1. Download `MLA_x64-setup.exe` and run it. Windows SmartScreen may show a warning because the app is not commercially code-signed — click **"More info" → "Run anyway"**.
2. On first start, a short setup guides you through language, name, AI model download and folder selection.

**Requirements:** Windows 10/11 (64-bit), 8 GB RAM minimum (16 GB recommended), ~10 GB free disk space for the app and one AI model.

### 🐧 Linux (beta)

1. Download `MLA_amd64.AppImage`, make it executable and run it:
   ```bash
   chmod +x MLA_*_amd64.AppImage
   ./MLA_*_amd64.AppImage
   ```
2. Requires `webkit2gtk-4.1` (preinstalled on most desktop distributions).

**Beta note:** Core features (chat, models, anonymization, knowledge chat) work; Windows-specific integrations (Task Scheduler jobs, autostart, global dictation hotkeys under Wayland) are still being ported.

## Privacy

Everything — AI models, speech recognition, your documents and notes — is processed locally on your machine. Internet access is used only for optional features (web search, model downloads, update check) and can be disabled completely with the built-in kill switch.

## License

© accola88. All rights reserved.

**Free to use** for personal purposes. Redistribution or modification requires permission. This application bundles open-source components — see `THIRD-PARTY-NOTICES.txt` included with the installation.
