# India Speaks - Scalable Indic-Language Audio-Text Preprocessing Pipeline

This project implements a robust preprocessing pipeline for multilingual audio-text data to prepare datasets for training TTS and ASR systems across 12+ Indic languages.

##  Features
- Audio path validation (stubbed as per task)
- Duration check (>15s rows flagged)
- Text normalization per IndiaSpeaks standards:
  - Unicode NFC normalization
  - Hindi digit expansion
  - Language-specific punctuation filtering
  - English lowercasing
  - Non-verbal token preservation
- Language mismatch detection using fastText
- Output: 
  - `train_ready.csv` with clean data
  - `rejected.csv` with rejected rows and reasons

##  Requirements
Install dependencies:
```bash
pip install -r requirements.txt
