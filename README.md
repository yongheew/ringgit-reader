# ringgit-reader
AI-powered Malaysian Ringgit banknote recognition for blind and visually impaired users, specifically for Malaysians. The core module is on-device Malaysian Ringgit (MYR) banknote recognition, which includes on-device computer vision with confidence-aware audio feedback. The user will point their phones at a note, and a lightweight computer vision model (YOLO/Mobile Net running locally via TensorFlow Lite or TensorFlow.js) identifies the denomination in real time and announces it through short audio cues, such as "fifty ringgit" using the phone's in-built TTS.


