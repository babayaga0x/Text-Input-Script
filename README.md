# ⌨️ Text Input Script

A Python automation script for typing speed tests and other text input scenarios.  
Uses `pyautogui` to simulate keyboard input automatically after a short delay.

---

## 📌 Description

**Text Input Script** is a lightweight Python tool that automatically types predefined text into any active input field. It's designed for typing speed tests — just set your text, click into the target field, and the script will start typing after a configurable countdown delay.

---

## 🧠 Features

- ⌨️ Simulates realistic keyboard input via `pyautogui`
- ⏱️ Configurable delay before typing starts
- 📝 Easily customizable input text directly in the script
- 🖱️ Works with any text field on screen — browser, desktop app, etc.
- 🪶 Minimal setup — single script, one dependency

---

## 🛠 Technologies Used

| Layer      | Technology     |
|------------|----------------|
| Language   | Python 3       |
| Automation | pyautogui      |

---

## 🚀 Quick Start

### Requirements

- Python 3.x
- pip

### Install Dependency
```bash
pip install pyautogui
```

### Clone the Repository
```bash
git clone https://github.com/babayaga0x/Text-Input-Script.git
cd Text-Input-Script
```

---

## ⚙️ Configuration

Open the script and edit the following variables before running:
```python
# The text that will be automatically typed
text = "Your text here"

# Delay in seconds before typing begins
delay_before_start = 10
```

---

## ▶️ Usage

1. Run the script:
```bash
python main.py
```

2. Within the countdown window (default **10 seconds**), click into the target text input field — browser typing test, desktop app, or any other input.

3. The script will automatically start typing the configured text once the delay expires.

---

## 💡 Use Cases

- 🏁 Automated typing speed tests (e.g. [typeracer.com](https://typeracer.com), [monkeytype.com](https://monkeytype.com))
- 🧪 Testing text input fields in web or desktop applications
- 🔁 Repeating text entry tasks automatically
- 📚 Learning Python automation with `pyautogui`

---

## ⚠️ Notes

- Make sure the target input field is **focused and active** before the delay runs out
- The script types at a set speed — adjust `pyautogui.typewrite()` interval if needed:
```python
pyautogui.typewrite(text, interval=0.05)  # seconds between keystrokes
```

- On **macOS**, you may need to grant accessibility permissions to your terminal in  
  `System Settings → Privacy & Security → Accessibility`
- On **Linux**, `pyautogui` may require `python3-xlib` or `python3-tk`:
```bash
pip install python3-xlib
# or
sudo apt install python3-tk python3-dev
```

---

## 📁 Project Structure
```
Text-Input-Script/
│
├── main.py       # Main script with text and delay configuration
└── README.md
```

---

## 📈 Roadmap

Potential future improvements:

- CLI arguments for text and delay (`--text`, `--delay`)
- Read input text from an external `.txt` file
- Adjustable typing speed (WPM-based)
- Support for multi-line text input

---

## 📄 License

MIT License


<p align="center">
  <img src="https://github.com/user-attachments/assets/69139c1a-f471-40eb-bf86-2ec93b3792e3" />
</p>
