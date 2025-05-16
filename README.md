🎙️ Comic-to-Audio Converter
Convert your comic book panels into speech using OCR and Text-to-Speech (TTS) technology!

This project automatically detects panels in a comic image, extracts text from each panel using EasyOCR, and generates corresponding audio files using Google Text-to-Speech (gTTS).
🎧 Finally, all panel audios are merged into a single audio file to give a seamless voiceover experience of the comic.

📌 Features
📖 Comic Panel Detection
– Automatically splits comic pages into individual panels.

🔍 Text Extraction
– Uses EasyOCR to extract text from each panel.

🎤 Text-to-Speech
– Converts panel text to speech using gTTS.

🎧 Audio Compilation
– Combines all audio files into one with pauses between panels.

🛠️ Installation
Make sure you're running this in a Python environment (e.g., Google Colab or local Jupyter Notebook).
Then install the dependencies:

bash
Copy
Edit
pip install easyocr opencv-python numpy matplotlib gTTS pydub
You also need to install FFmpeg for pydub to work correctly.
In Google Colab, run:

bash
Copy
Edit
!apt install ffmpeg
🚀 How to Use
➕ Add your comic image
Place your comic image in the working directory and update the path:

python
Copy
Edit
image_path = "Comic3.jpg"
▶️ Run the main process
This will:

✅ Detect comic panels

✅ Extract text

✅ Generate TTS for each panel

✅ Save all panel audios

✅ Merge them into a single audio file

🧠 How It Works
🖼️ Panel Detection
Converts the comic to binary using thresholding.

Detects horizontal and vertical whitespace to segment panels.

👁️ OCR
Uses EasyOCR to read English text from each panel image.

🔊 Text-to-Speech
Uses Google Text-to-Speech (gTTS) to generate MP3 files.

🎚️ Audio Merging
Uses pydub to concatenate all panel audio files with short pauses in between.

📌 Dependencies
EasyOCR

OpenCV

NumPy

Matplotlib

gTTS

pydub

📄 License
This project is open-source under the MIT License.

🙌 Acknowledgments
Comic image used is for demonstration only.

TTS powered by gTTS

OCR by EasyOCR

