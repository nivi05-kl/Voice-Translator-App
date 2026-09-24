
# 🎙️ Voice Translator — English ↔ Tamil

> A simple voice-based translation app built with **MIT App Inventor** that helps users speak in English or Tamil, translate the speech, and hear the translated result aloud.

<p align="center">
  <img src="assets/voice-translator-app.png" alt="Voice Translator App" width="300">
</p>

<p align="center">
  <b>English → Tamil</b> &nbsp; • &nbsp; <b>Tamil → English</b> &nbsp; • &nbsp; <b>Speech Recognition</b> &nbsp; • &nbsp; <b>Text-to-Speech</b>
</p>

---

## 📌 About the Project

**Voice Translator** is a beginner-friendly mobile application created using **MIT App Inventor**.

The app focuses on making language translation easier through voice input. Instead of typing a sentence, the user can select a language, speak into the microphone, and receive a translated response. The translated text can also be spoken aloud.

This project demonstrates how visual programming can be used to combine:

- 🎤 Speech recognition
- 🌐 Language translation
- 🔊 Text-to-speech
- 🧩 Event-driven programming
- 📱 Mobile app UI design

---

## ✨ Features

| Feature | Description |
|---|---|
| 🇬🇧 English → Tamil | Speak in English and translate it into Tamil |
| 🇮🇳 Tamil → English | Speak in Tamil and translate it into English |
| 🎤 Voice Input | Uses the phone microphone through SpeechRecognizer |
| 🌐 Translation | Uses the Translator component |
| 🔊 Voice Output | Reads the translated sentence using TextToSpeech |
| 🖥️ Simple UI | Designed to be easy for a student/user to understand |
| 🔄 Two-way Translation | Supports both language directions |

---

## 🛠️ Technology Used

- **MIT App Inventor**
- **SpeechRecognizer**
- **Translator**
- **TextToSpeech**
- **Event-driven Blocks**
- **Android**

### Main Components

```text
SpeechRecognizer
      ↓
Recognized Speech
      ↓
Translator
      ↓
Translated Text
      ↓
TextToSpeech
```

---

## 🧩 How the App Works

### 1. English Button

When the user selects **English**:

```text
Language = en-US
        ↓
SpeechRecognizer.GetText
        ↓
Recognized English speech
        ↓
Translate to Tamil
```

### 2. Tamil Button

When the user selects **Tamil**:

```text
Language = ta-IN
        ↓
SpeechRecognizer.GetText
        ↓
Recognized Tamil speech
        ↓
Translate to English
```

### 3. Translation Result

The `AfterGettingText` event checks which language is selected and sends the recognized speech to the Translator component.

### 4. Voice Output

After translation is completed:

```text
Translation received
        ↓
Display translated text
        ↓
TextToSpeech.Speak
```

---

## 🧠 Block Logic

The app uses a global variable called `Lang` to remember the selected input language.

```text
Lang = 1  → English input
Lang = 0  → Tamil input
```

The main event flow is:

```text
User selects language
        ↓
Set SpeechRecognizer language
        ↓
Start speech recognition
        ↓
AfterGettingText
        ↓
Check Lang
        ↓
Request translation
        ↓
GotTranslation
        ↓
Show translated text
        ↓
Speak translated text
```

<p align="center">
  <img src="assets/voice-translator-blocks.png" alt="MIT App Inventor Blocks" width="700">
</p>

---

## 📱 App Preview

### Voice Translator Home Screen

The interface presents the project as a simple voice-translation experience with a microphone-themed visual design.

<p align="center">
  <img src="assets/voice-translator-app.png" alt="Voice Translator mobile screen" width="280">
</p>

---

## 🎯 Project Objective

The main objective of this project is to create a simple application that can:

1. Accept speech from the user.
2. Recognize the spoken language.
3. Translate the recognized text.
4. Display the translated text.
5. Convert the translated text back into speech.

This project was also created to understand how different app components can work together through **MIT App Inventor blocks**.

---

## 🚀 How to Run the Project

### Option 1 — MIT App Inventor

1. Open **MIT App Inventor**.
2. Create/open the Voice Translator project.
3. Add the required components:
   - SpeechRecognizer
   - Translator
   - TextToSpeech
   - Buttons
   - Labels
   - Image/background elements
4. Recreate/import the blocks shown in the project.
5. Test the application using an Android phone or emulator.

### Permissions

The app needs microphone access for speech recognition.

> Translation and speech recognition may require an internet connection depending on the component/service and device configuration.

---

## 📂 Suggested GitHub Repository Structure

```text
Voice-Translator/
│
├── README.md
│
├── assets/
│   ├── voice-translator-app.png
│   └── voice-translator-blocks.png
│
└── VoiceTranslator.aia
```

If you have the MIT App Inventor `.aia` project file, add it to the repository using the name:

```text
VoiceTranslator.aia
```

---

## 🔮 Future Improvements

Possible improvements for a future version:

- 🌍 Add more languages
- 🕘 Add translation history
- 📋 Add copy-to-clipboard
- 🗑️ Add clear/reset button
- 🎨 Add dark mode
- 🔊 Add speech speed controls
- ⭐ Save frequently used translations
- 📶 Show an internet/network status
- 🗣️ Improve language selection with a dropdown menu

---

## 📚 What I Learned

Through this project, I practiced:

- Designing a mobile application using MIT App Inventor
- Working with event-driven programming
- Using speech recognition
- Passing data between components
- Using translation services
- Using text-to-speech
- Creating conditional logic with blocks
- Building a practical application from a real-world idea

---

## 👩‍💻 Project Type

**Academic / Student Mini Project**

**Platform:** Android  
**Development Tool:** MIT App Inventor  
**Project Area:** Mobile Application Development + Language Technology

---

## ⭐ If You Like This Project

Feel free to ⭐ star the repository and use the project as a learning reference for MIT App Inventor.

---

## 📄 License

This project is intended for educational and learning purposes.
