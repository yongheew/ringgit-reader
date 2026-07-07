# Ringgit Reader 💰
AI-powered Malaysian Ringgit banknote recognition for blind and visually impaired users, specifically for Malaysians. The core module is on-device Malaysian Ringgit (MYR) banknote recognition, which includes on-device computer vision with confidence-aware audio feedback. The user will point their phones at a note, and a lightweight computer vision model (YOLO/Mobile Net running locally via TensorFlow Lite or TensorFlow.js) identifies the denomination in real time and announces it through short audio cues, such as "fifty ringgit" using the phone's in-built TTS.

## Key Design Principles 🔑
* Localized: Trained on self-collected dataset of real ringgit notes: worn, crumpled, folded... etc.
* Confidence-aware: Only announces to user after stable, high confidence detections across consecutive frames; if uncertain, it says "hold steady" instead of guessing.
* Instant and offline: No internet needed, on-device inference
* Evakuate properly: Accuracy, false-positive rate, and latency measured under varied real-world conditions

## Planned Extensions 📂
* DuitNow QR standee locator: With audio aiming guidance, VLM-based scene description on demand, and AI-to-human volunteer handoff for uncertain situations, such as positioning the currency module.
