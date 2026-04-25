🤖 Xiaozhi AI Voice Bot (Custom PCB Version)
📌 Overview

This project is a custom hardware implementation of an ESP32-based AI voice assistant inspired by the Xiaozhi-ESP32 project.

Unlike a standard breadboard setup, I designed and built a compact PCB integrating audio, power, and control systems to create a standalone conversational device.

🎯 Features:
1.🎤 Voice input using I2S microphone
2.🔊 Audio output via I2S amplifier + speaker
3.🌐 WiFi-based communication with AI server
4.🧠 Real-time voice interaction (Speech → AI → Speech)
5.🔘 Physical buttons for interaction control
6.⚡ Custom PCB for compact and stable design
7.🧠 How It Works (My Understanding)

This system does NOT run AI locally. Instead, it works as a smart client:

1.ESP32 captures voice input through microphone
2.Audio is sent to a server over WiFi
3.Server performs:
4.Speech-to-Text (STT)
5.AI processing (LLM)
6.Text-to-Speech (TTS)
7.Processed audio is sent back
8.ESP32 plays response via speaker

This creates a real-time conversational loop.

🛠️ Hardware Design
Components Used:
1.ESP32 (XIAO ESP32-S3)
2.I2S Microphone (INMP441)
3.I2S Amplifier (MAX98357A)
3.Speaker
4.Push Buttons

🔧 PCB Design:

I designed a custom PCB to:

1.Reduce wiring complexity
2.Improve stability
3.Make the device portable

🔥 Soldering Process
1.Soldered SMD and through-hole components manually
2.Ensured proper grounding for audio clarity
3.Carefully routed I2S lines to avoid noise issues
