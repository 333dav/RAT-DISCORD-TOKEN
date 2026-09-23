
# ⚙️ Remote Control Panel via Chat (Discord Bot)

> ⚠️ **IMPORTANT WARNING:** This project was developed strictly for **educational purposes and study in personal laboratory environments (homelabs)**. The author is not responsible for any misuse, damage, or illegal activities carried out with this code. Use responsibly only on systems you own or have express authorization to access.

---

## 🛠️ Initial Configuration

Before running the application, you **must configure** your credentials in the `rat.py` file. The code features a built-in safety check (Fail-safe) that prevents execution if the default values are left unchanged.

Open the `rat.py` file and modify the following lines with your data:

```python
BOT_TOKEN = "YOUR_API_TOKEN_HERE"       # Replace with your Discord Bot Token
CHANNEL_ID = 123456789012345678        # Replace with your Discord channel numeric ID (integer)
```

> ⚠️ **Note:** If you forget to change these variables, the script will trigger a Windows error message box (`Configuration Error`) and terminate execution immediately.

---

## 🚀 Compiling to Executable (.exe)

To transform your Python script into a standalone executable file (which runs without requiring Python installed on the target host), run the following command in your VS Code terminal:

```bash
python -m PyInstaller --onefile --windowed YourFileName.py
```

### 💡 Parameter Breakdown:
* **`--onefile`**: Bundles the entire project and its dependencies into a single `.exe` file.
* **`--windowed`**: Hides the black console window (Command Prompt) when launching the application.

---

## 📋 Available Commands

Below is the complete list of commands organized by category for easier host administration.

### 🛠️ System & Navigation
* **`!help`**: Displays the full list of all available options and commands.
* **`!startup`**: Adds the executable to the Windows startup registry (Autostart).
* **`!execute <commands>`**: Runs a command directly in the shell (Terminal/Command Prompt).
* **`!cd <directory>`**: Changes the bot's current working directory.
* **`!openlink <url>`**: Opens a specific URL in the system's default browser (Chrome/Opera/Edge).

### 📊 Processes & Information
* **`!process`**: Lists all active processes currently running on the target machine.
* **`!processkill <pid>`**: Terminates a specific process using its Process ID (PID).
* **`!ip`**: Fetches detailed information about the machine's current public IP address.
* **`!sysinfo`**: Gathers and displays detailed system technical specifications.

### 📂 File Transfer
* **`!download <file_name>`**: Downloads a file located on the host computer.
* **`!upload`**: Uploads a file to the host computer (you must attach the file along with the command).

### 🔍 Monitoring & Capture
* **`!keylog`**: Starts monitoring and recording keystrokes (Keylogger).
* **`!stoplog`**: Stops the Keylogger and retrieves the file containing the typed history.
* **`!screenshot`**: Captures a real-time screenshot of the host computer's current display.
* **`!webcam`**: Captures a snapshot/photo from the webcam connected to the device.

### 🔐 Data Extraction (Dump)
* **`!password`**: Decrypts and displays stored passwords saved on the system.
* **`!autofill`**: Extracts autofill profiles and credit cards saved in browsers.

### ⚠️ Power Actions & Interface
* **`!wallpaper`**: Changes the desktop background (requires attaching a file or providing an image URL).
* **`!shutdown`**: Shuts down the target computer's operating system immediately.
* **`!restart`**: Restarts the target computer's operating system immediately.
* **`!bsod`**: Forces a native Blue Screen of Death (BSOD) on Windows.

---

## 📦 Dependencies & Prerequisites

To run and compile this script, you will need to install the required libraries:

```bash
# Installs the default bot dependencies and the compiler
pip install discord.py pyinstaller
```

---

<div align="center">

<h3>🐉 Made by dav 🐉</h3>

[![GitHub](https://shields.io)](https://github.com/333dav)

</div>
