
# 🎙️ Python TTS Button App

This is a floating Text-to-Speech (TTS) button built with Python and Tkinter using `ttkbootstrap`. It lets you type text in Spanish and outputs the spoken audio through **VB-Audio Virtual Cable**, which you can route into apps like **Discord**, **OBS**, or **Voicemeeter**.

---

## 🧰 Features

- Floating draggable 🔊 button always on top
- Opens a minimal textbox popup to type speech
- Uses **Google TTS** (gTTS)
- Sends audio to **VB-Audio Virtual Cable** for routing
- Automatically opens and minimizes **Voicemeeter Banana**

---

## 🚀 Requirements

### 1. Python Packages

Install required libraries with:

```bash
pip install gTTS sounddevice soundfile numpy pygetwindow pywin32 ttkbootstrap
```

### 2. Voicemeeter Banana (REQUIRED)

Download and install Voicemeeter Banana from the official website:

🔗 https://vb-audio.com/

This app launches and minimizes Voicemeeter automatically. Ensure it's installed in this path:

```
C:\Program Files (x86)\VB\Voicemeeter\voicemeeterpro_x64.exe
```

If your install path is different, edit the `vm_path` in the script.

### 3. VB-CABLE (REQUIRED)

VB-CABLE is used to route the voice output to Discord, OBS, or other apps.

Download and install it here:

🔗 https://vb-audio.com/

After installing:
- Set **VB-CABLE** as the output device in the script (it's already configured by default).
- Set **VB-CABLE** as input in VoiceMeeter Banana.
- Set **VoiceMeeter Out B1** as the input in Discord.
---

## 📦 Project Structure

```
TextSpeech/
│
├── ttsv2.py         # Main Python script
├── VoicemeeterRemote.dll
├── VoicemeeterRemote64.dll
└── README.md       # Project instructions
```

---

## 💬 How to Use

1. Run the script:
    ```bash
    python main.py
    ```
2. A draggable button will appear.
3. Click the button to open a textbox popup.
4. Type your message and press **Enter** to play the voice through **VB-CABLE**.
5. Press **ESC** to close the textbox popup.
6. Right click the button to display the exit option and close the app.

---

## 🛠️ Customization

- Default language is Spanish (`lang='es'` in `gTTS`). Change to `'en'`, `'fr'`, etc. as needed.
- Button and window are styled with `ttkbootstrap`. You can modify the theme and layout.
- Add shortcuts, system tray icon, or speech presets for more features.

---

## 🧠 Use Cases

- Voice chat in Discord using TTS
- Broadcasting messages in OBS
- Fun or accessibility tool

---

Enjoy! 🎧
