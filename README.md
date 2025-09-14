# Audio Recorder ALT Version

This is an alternative implementation of the Audio Recorder application, featuring a clean HTML-based interface for recording audio directly in the browser.

## Features

- **Microphone Recording**: Record audio from your device's microphone
- **Real-time Level Meter**: Visual feedback showing audio input levels during recording
- **MP3 Conversion**: Automatic conversion of recorded audio to MP3 format using lamejs
- **Auto Download**: Recorded MP3 files are automatically downloaded to your Downloads folder
- **Timer Display**: Shows recording duration in MM:SS format
- **Responsive Design**: Works on desktop and mobile devices

## Usage

1. Open `audio-recorder.html` in a modern web browser that supports `getUserMedia` (Chrome, Firefox, Safari, Edge)
2. Click the "Record" button to start recording
3. Click the "Stop" button to end recording and download the MP3 file
4. The recording will be saved as `recording_YYYY-MM-DDTHH-MM-SS.mp3` in your Downloads folder

## Dependencies

- **lamejs**: MP3 encoding library (loaded via CDN from https://cdn.jsdelivr.net/npm/lamejs@1.2.0/lame.min.js)

## Browser Requirements

- Modern browser with Web Audio API support
- Microphone access permission
- HTTPS connection (required for microphone access in most browsers)

## Technical Details

- Uses MediaRecorder API for audio capture
- Web Audio API for real-time level analysis
- Client-side MP3 encoding with lamejs
- No server-side processing required

## Privacy

All audio recording and processing is performed entirely on your local machine. No audio data is transmitted to remote servers. The lamejs library is loaded from a CDN for MP3 encoding, but your recorded audio never leaves your device.

## Note

This ALT version removes the original `index.html` and focuses solely on the `audio-recorder.html` implementation for a streamlined experience.
