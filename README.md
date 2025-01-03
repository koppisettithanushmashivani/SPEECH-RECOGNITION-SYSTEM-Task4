# SPEECH-RECOGNITION-SYSTEM-Task4

**COMPANY**: CODTECH IT SOLUTIONS
**NAME**: KOPPISETTI THANUSHMA SHIVANI
**INTERN ID**:CT12EGF
**DOMAIN**: EMBEDDED SYSTEMS
**BATCH DURATION**:DECEMBER 17th, 2025 TO FEBURARY 17th, 2025
**MENTOR NAME**:NEELA SANTOSH KUMAR

# DESCRIPTION OF THE TASK

OBJECTIVE:
   The objective of a Speech Recognition System is to enable command-based control of devices through voice input, providing a hands-free and intuitive user interface. This system leverages speech recognition technology to process spoken commands, interpret them, and trigger corresponding actions on connected devices. Implemented using an embedded board, it demonstrates the practical application of voice control in modern automation. The system aims to enhance user convenience, improve accessibility, and reduce reliance on physical controls, making it suitable for smart home applications, industrial automation, and assistive technologies.

INTRODUCTION:
  A Speech Recognition System is an innovative technology designed to enable devices to interpret and respond to spoken commands. By building a basic speech recognition system, users can control devices seamlessly using their voice, eliminating the need for physical interaction. This system, implemented with an embedded board, processes audio input, converts it into text or commands, and triggers the corresponding actions on connected devices. It represents a significant step towards creating intuitive and accessible human-machine interfaces, finding applications in smart homes, assistive technologies, and industrial automation. This system demonstrates the potential of voice-based control in enhancing user convenience and interaction.

KEY ACTIVITIES:
1.Audio Input Capture:
Use a microphone to capture spoken commands.

2.Signal Processing:
Convert the captured audio signals into a digital format for processing by the embedded board.

3.Speech Recognition:
Use a speech recognition module or software to analyze and recognize the spoken words or commands.

4.Command Interpretation:
Interpret the recognized commands into actionable instructions.

5.Device Control:
Trigger corresponding actions on the connected devices based on the recognized commands.

6.Calibration:
Fine-tune the system to accurately recognize specific commands or keywords.

7.Power Management:
Ensure stable power supply and efficient operation of the embedded system.

8.System Integration:
Integrate the embedded board with the devices for seamless control and communication.

9.Communication Protocols:
Set up communication channels (e.g., Bluetooth, Wi-Fi) between the embedded system and devices.

SOURCE CODE:
import speech_recognition as sr

# Initialize recognizer class (for recognizing the speech)
r = sr.Recognizer()

# Reading Microphone as source
# listening the speech and store in audio_text variable
with sr.Microphone() as source:
    print("Talk")
    audio_text = r.listen(source)
    print("Time over, thanks")
    # recoginze_() method will throw a request
    # error if the API is unreachable,
    # hence using exception handling
    
    try:
        # using google speech recognition
        print("Text: "+r.recognize_google(audio_text))
    except:
         print("Sorry, I did not get that")

  SYSTEM DESIGN:https://github.com/koppisettithanushmashivani/SPEECH-RECOGNITION-SYSTEM-Task4/commit/0304965cb3ff9033cd358d65fe953d5ec1a42ec4

  WORKING:
    The Speech Recognition System operates by capturing spoken commands through a microphone, which serves as the audio input. The embedded board processes these audio signals, converting them into a digital format suitable for analysis. A speech recognition module or algorithm on the board interprets the digital audio, identifying specific keywords or phrases that correspond to predefined commands. Once the commands are recognized, the system translates them into control signals that trigger actions on connected devices, such as turning a light on or off or adjusting a thermostat. This process occurs in real time, ensuring seamless and efficient device control. Additional features, like noise filtering and keyword detection, enhance the system's accuracy and reliability, making it a practical solution for hands-free command-based automation.

CONCLUSION:
  In conclusion, the Speech Recognition System provides a practical and efficient solution for command-based control of devices using voice input. By integrating a microphone, embedded board, and speech recognition technology, the system enables seamless and hands-free operation, enhancing user convenience and accessibility. Its ability to interpret spoken commands and execute corresponding actions in real time demonstrates its potential in smart automation, assistive technologies, and industrial applications. This system highlights the power of voice-controlled interfaces in creating intuitive and interactive environments, paving the way for future advancements in human-machine interaction.


OUTPUT OF THE PROJECT:








