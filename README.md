🤖 Xiaozhi AI Voice Bot (Custom PCB Version)
📌 Overview

This project is a custom hardware implementation of an ESP32-based AI voice assistant inspired by the Xiaozhi-ESP32 project.

Unlike a standard breadboard setup, I designed and built a compact PCB integrating audio, power, and control systems to create a standalone conversational device.

🎯 Features
🎤 Voice input using I2S microphone
🔊 Audio output via I2S amplifier + speaker
🌐 WiFi-based communication with AI server
🧠 Real-time voice interaction (Speech → AI → Speech)
🔘 Physical buttons for interaction control
⚡ Custom PCB for compact and stable design
🧠 How It Works (My Understanding)

This system does NOT run AI locally. Instead, it works as a smart client:

ESP32 captures voice input through microphone
Audio is sent to a server over WiFi
Server performs:
Speech-to-Text (STT)
AI processing (LLM)
Text-to-Speech (TTS)
Processed audio is sent back
ESP32 plays response via speaker

This creates a real-time conversational loop.

🛠️ Hardware Design
Components Used:
ESP32 (XIAO ESP32-S3)
I2S Microphone (INMP441)
I2S Amplifier (MAX98357A)
Speaker
Push Buttons
Power Regulation Circuit
🔧 PCB Design

I designed a custom PCB to:

Reduce wiring complexity
Improve stability
Make the device portable

(Insert PCB images here)

🔥 Soldering Process
Soldered SMD and through-hole components manually
Ensured proper grounding for audio clarity
Carefully routed I2S lines to avoid noise issues
