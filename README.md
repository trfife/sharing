# Transcription Watcher

Automatically captures Teams Live Captions to a text file — no setup, no permissions, no Graph API needed.

## Getting Started

1. **Unzip** the folder and run **`TranscriptionWatcher.exe`**
2. A blue icon appears in your **system tray** (bottom-right of your taskbar — you may need to click the `^` arrow to see it)
3. That's it — it's now watching for captions in the background

> **No Python or other software is required.** Just run the exe.

## How to Capture a Meeting

### Step 1: Turn on Live Captions in Teams

During a Teams meeting:

1. Click **More** (`···`) in the meeting toolbar
2. Go to **Language and speech**
3. Click **Show live captions**

A captions bar will appear at the bottom of your Teams window.

### Step 2: Open Captions in a New Window

On the captions bar at the bottom of Teams, click the **"Open captions in new window"** button (the small pop-out icon in the top-right corner of the captions panel).

This opens captions in a separate window titled **"Captions | Meeting Name"**.

### Step 3: It Just Works

Once the captions window is open, Transcription Watcher:

- **Automatically detects** the captions window
- **Moves it to the background** so it's out of your way
- **Captures everything** with speaker names and timestamps
- **Saves to a text file** when the meeting ends

You'll see a Windows notification confirming capture has started.

## Where Are Transcripts Saved?

Transcripts are saved to:

```
Documents\OneDrive - Microsoft\Squad\Transcriptions\
```

Each file is named: `Meeting Name - YYYY-MM-DD.txt`

## System Tray Menu

Right-click the blue tray icon for options:

| Option | What it does |
|---|---|
| **Open** | Shows the main Transcription Watcher window |
| **Open Last Transcript** | Opens the most recently saved transcript file |
| **Quit** | Exits the application |

## Auto-Delete

Transcripts are **automatically deleted 10 minutes** after the meeting ends. If you want to keep a transcript, open it from the tray menu and save a copy before the timer expires.

## Tips

- You can leave Transcription Watcher running all day — it will automatically capture every meeting where you open live captions
- If you rejoin the same meeting, it appends to the same daily file
- The captions window can be minimized — capture still works
- Speaker names are detected automatically when Teams provides them

## Requirements

- Windows 10 or 11 (64-bit)
- Microsoft Teams desktop app
