# Godrick

Godrick is a terminal workspace for coding agents on Windows. It runs agents in split panes, lets a Chief delegate work into separate Git worktrees, and gives you a review step before each merge.

## Get started

1. Download the Windows x64 ZIP from [Releases](https://github.com/Khaile31/godrick/releases/latest) and extract it.
2. In PowerShell, go to the extracted directory and run `.\godrick.exe`. Godrick uses Windows Terminal or another compatible console.
3. Press `1` for Chief, `2` for terminal panes, and `4` to review changes. In Chief, press `i` to write and `Enter` to send.

Install Git and a supported coding CLI to delegate coding tasks. You can register an existing repository from PowerShell.

```powershell
.\godrick.exe project add 'C:\path\to\repo' --test 'cargo test'
.\godrick.exe
```

Press `q` to close the interface while the agents continue. Run `.\godrick.exe daemon stop` to stop the background process and its agents.

Godrick starts with its own state directory under `%LOCALAPPDATA%\godrick`. Existing Hivemux sessions stay in their original state directory. A separate release asset provides the ZIP's SHA-256 checksum. The Windows executable is unsigned.

Godrick is distributed under the Apache License 2.0. The ZIP includes third-party license notices.
