# 🎙️ Comic-to-Audio Converter

Convert your comic book panels into speech using OCR and Text-to-Speech (TTS) technology!

This project automatically detects panels in a comic image, extracts text using [EasyOCR](https://github.com/JaidedAI/EasyOCR), and generates corresponding audio using [gTTS](https://pypi.org/project/gTTS/). Finally, it merges the panel audios into a single voiceover file for a seamless listening experience.

---

## 📌 Features

- 📖 **Comic Panel Detection**  
  Automatically splits comic pages into individual panels using image processing.

- 🔍 **Text Extraction**  
  Extracts English text from each panel using EasyOCR.

- 🎤 **Text-to-Speech**  
  Converts extracted text to audio using Google Text-to-Speech (gTTS).

- 🎧 **Audio Compilation**  
  Combines all panel audio files into one, with pauses between them.

---

## 🛠️ Installation

Ensure you're using a Python environment like Google Colab or Jupyter Notebook. Then install the dependencies:

```bash
pip install easyocr opencv-python numpy matplotlib gTTS pydub
```
Also, install FFmpeg for audio processing via pydub.
In Google Colab, run:
```bash
!apt install ffmpeg
```
## 🚀 How to Use

### ➕ Add Your Comic Image

- Place your comic image in the working directory.
- Update the path in the code:

```python
image_path = "Comic3.jpg"
```
### ▶️ Run the Main Process
This will:

- ✅ Detect comic panels  
- ✅ Extract text from each panel  
- ✅ Generate TTS for each panel  
- ✅ Save panel audios  
- ✅ Merge them into a single audio file  

---

### 🧠 How It Works

#### 🖼️ Panel Detection
- Converts comic image to binary using thresholding.
- Identifies white spaces to segment panels.

#### 👁️ OCR
- Uses EasyOCR to extract text from each panel image.

#### 🔊 TTS
- Uses Google Text-to-Speech (gTTS) to convert text to MP3 files.

#### 🎚️ Audio Merging
- Uses pydub to concatenate all MP3s with short pauses in between.

---

### 📦 Dependencies

- easyocr  
- opencv-python  
- numpy  
- matplotlib  
- gTTS  
- pydub  

**System Dependency:**  
- ffmpeg (external system dependency)

---

### 📄 License
This project is licensed under the **MIT License**.  

---

### 🙌 Acknowledgments

- Comic images used are for demonstration purposes only.  
- OCR by **EasyOCR**  
- TTS powered by **gTTS**
