# **Jarvis AI Assistant - README**

## **Overview**
This project is a simple voice-controlled AI assistant named *Jarvis* that can perform various tasks such as:
- Speaking the current time and date
- Performing web searches
- Sending emails
- Taking screenshots
- Telling jokes
- Monitoring CPU and battery usage
- Playing music
- Shutting down or restarting your system

The assistant uses speech recognition, text-to-speech, and automation libraries in Python.

---

## **Installation**

Before running the project, ensure you have Python installed. Then, install the required libraries:

```bash
pip install pyttsx3
pip install SpeechRecognition
pip install pyaudio
pip install wikipedia
pip install pyautogui
pip install psutil --upgrade
pip install pyjokes
```

---

## **Dependencies**
The following Python libraries are used:
1. **pyttsx3** - Text-to-speech conversion
2. **SpeechRecognition** - Recognizes speech input
3. **pyaudio** - Enables audio input/output
4. **wikipedia** - Fetches information from Wikipedia
5. **pyautogui** - Automates GUI tasks (e.g., screenshots)
6. **psutil** - Monitors CPU and battery usage
7. **pyjokes** - Fetches random jokes

---

## **How to Run**

1. **Save the Script**: Copy the code into a Python file, e.g., `jarvis.py`.
2. **Run the Script**:
   Open a terminal and execute:
   ```bash
   python jarvis.py
   ```
3. **Interact with Jarvis**: Use voice commands such as:
   - "What is the time?"
   - "Tell me a joke."
   - "Take a screenshot."
   - "Search in Chrome."
   - "Play songs."
   - "Shutdown" or "Restart" system.
   - "Remember that..." and "Do you know anything?"

---

## **Features**

1. **Time and Date**:
   Jarvis speaks out the current time and date.

2. **Wikipedia Search**:
   - Command: "Search [topic] on Wikipedia."
   - Jarvis fetches a brief summary from Wikipedia.

3. **Email Sending**:
   - Command: "Send email."
   - You can dictate the content, and it sends an email.

4. **System Commands**:
   - Logout, Shutdown, Restart.

5. **Music Playback**:
   - Plays the first song in a specified directory.

6. **Take Notes**:
   - Command: "Remember that..."
   - Jarvis remembers and recalls notes.

7. **Screenshot**:
   - Command: "Take a screenshot."
   - Saves a screenshot to a specified location.

8. **System Monitoring**:
   - Command: "CPU."
   - Jarvis reports CPU usage and battery status.

9. **Jokes**:
   - Command: "Tell me a joke."

10. **Web Search**:
    - Command: "Search in Chrome."

11. **Quit**:
    - Command: "Go offline."

---

## **Customisation**

### **Email Configuration**
Replace the following with your Gmail credentials in the `sendEmail()` function:
```python
server.login('your_email@gmail.com', 'your_password')
```
**Note**: Enable "Less secure apps" in your Gmail settings for this to work.

### **Music Directory**
Update the path to your music folder:
```python
songs_dir = 'D:\\Music'
```

### **Screenshot Save Path**
Update the location where screenshots are saved:
```python
img.save("C:\\path_to_save\\screenshot.png")
```

---

## **Known Issues**
- **pyaudio Installation**: On some systems, installing `pyaudio` may require additional setup. Use the following:
   - For Windows:
     ```bash
     pip install pipwin
     pipwin install pyaudio
     ```
   - For Linux:
     ```bash
     sudo apt-get install portaudio19-dev
     pip install pyaudio
     ```

---

## **Future Improvements**
- Integrate with APIs for weather updates and news.
- Add voice authentication for security.
- Enhance conversation capabilities with NLP models.

---

## **Credits**
This project was developed by **Elijah Charles Enyi**.
