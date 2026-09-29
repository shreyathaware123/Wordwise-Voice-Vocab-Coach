# WordWise — Voice Vocabulary Coach

A simple voice agent that helps users practice new vocabulary out loud. It speaks a word, its meaning, and an example sentence, then listens as the user tries using the word in their own sentence and gives instant feedback.

🔗 **Live demo:** https://hilarious-heliotrope-f23f0b.netlify.app/

## Features
- Speaks each word, its meaning, and an example sentence (text-to-speech)
- Listens to the user's spoken sentence and checks if the word was used correctly (speech recognition)
- Gives instant spoken + on-screen feedback
- Falls back to a text input box if voice isn't supported or the mic doesn't catch clearly
- Tracks progress across 8 words with a final score

## Tech Used
Built as a single self-contained HTML/CSS/JavaScript page using the browser's native **Web Speech API**:
- `SpeechSynthesisUtterance` for text-to-speech
- `SpeechRecognition` / `webkitSpeechRecognition` for voice input

No backend, no paid API, no framework — runs entirely client-side.

## How to Run Locally
1. Clone this repo
2. Open `index.html` directly in Chrome (recommended for full voice support)
3. Allow microphone access when prompted

## Notes
- Works best in Chrome (desktop or Android) due to browser support for the Web Speech API.
- Safari/Firefox have limited or no speech recognition support — the app automatically switches to a typed-answer fallback in that case.
