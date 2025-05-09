# Chord Detector Chrome Extension

A powerful Chrome extension that detects musical chords in real-time from any audio source playing in your browser. Whether you're learning songs, transcribing music, or analyzing harmonies, this extension helps you identify chords as they play.

## Features

- **Real-time Chord Detection**: Analyzes audio in real-time using advanced frequency analysis and pattern matching
- **Wide Chord Recognition**: Detects various chord types:
  - Major chords (e.g., C, G, D)
  - Minor chords (e.g., Am, Em)
  - Diminished chords (e.g., Bdim)
  - Seventh chords (Major 7, Dominant 7, Minor 7)
- **Customizable Settings**:
  - Adjustable sensitivity threshold
  - Bass boost control
  - Frequency range customization
  - Update interval control
  - Chord type filtering
- **High Accuracy**: Uses sophisticated audio processing algorithms including:
  - FFT (Fast Fourier Transform) analysis
  - Chroma vector calculation
  - Pattern matching with chord templates
  - Bass note detection for improved accuracy

## Technical Details

### Audio Processing

- FFT Size: 8192 samples for high-resolution frequency analysis
- Frequency Range: 60Hz (B1) to 5000Hz (D#8)
- Update Interval: 150ms default, adjustable
- Chroma Smoothing: 6-frame window for stable detection

### Advanced Features

- **Bass Note Detection**: Specialized analysis below 220Hz for accurate bass note identification
- **Frequency Weighting**: Optimized for various instruments
  - Enhanced bass response (below 250Hz)
  - Balanced mid-range handling
- **Chord Recognition**: Uses cosine similarity matching against ideal chord templates
- **Temporal Smoothing**: Implements a chord buffer system to reduce fluctuations

## Installation

1. Clone this repository or download the source code
2. Open Chrome and navigate to `chrome://extensions/`
3. Enable "Developer mode" in the top right
4. Click "Load unpacked" and select the extension directory

## Usage

1. Click the extension icon in your Chrome toolbar
2. Grant audio capture permissions when prompted
3. Play audio from any tab in your browser
4. Watch as chords are detected and displayed in real-time

## Permissions

This extension requires:
- Audio capture permission for the active tab
- Access to tab audio for processing

## Privacy

- All audio processing is done locally in your browser
- No audio data is recorded or transmitted
- No external servers are contacted

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.

## License

MIT License - feel free to use and modify as needed.
