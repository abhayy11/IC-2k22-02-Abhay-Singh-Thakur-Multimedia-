# Multimedia Lab
# Multimedia Processing and Analysis Suite

A collection of Python-based multimedia projects developed as part of the **Multimedia Systems** coursework. This repository explores different aspects of digital multimedia processing, including image enhancement, image analysis, audio analysis, video analysis, and AI-powered voice cloning.

The projects demonstrate how Python libraries, computer vision techniques, image processing algorithms, audio-processing tools, and AI models can be used to process and analyze different forms of digital media.

---

## 📌 Table of Contents

1. [Project Overview](#-project-overview)
2. [Projects](#-projects)
   - [Image Enhancement and Text Extraction](#1-image-enhancement-and-text-extraction)
   - [Audio Analyzer](#2-audio-analyzer)
   - [Image Analyzer](#3-image-analyzer)
   - [Video Analyzer](#4-video-analyzer)
   - [Voice Cloning](#5-voice-cloning)
3. [Technologies Used](#-technologies-used)
4. [Repository Structure](#-repository-structure)
5. [Installation and Setup](#-installation-and-setup)
6. [Applications](#-real-world-applications)
7. [Learning Outcomes](#-learning-outcomes)
8. [Author](#-author)

---

## 🚀 Project Overview

This repository consists of five independent multimedia applications, each focusing on a different area of multimedia computing.

| Project | Description | Primary Technology |
|---|---|---|
| Image Enhancement and Text Extraction | Improves image quality and extracts text from images | OpenCV, EasyOCR |
| Audio Analyzer | Analyzes audio files and extracts audio information | Python, FFmpeg |
| Image Analyzer | Processes images and analyzes their properties | Python, Image Processing |
| Video Analyzer | Analyzes video files and their multimedia properties | Python, Video Processing |
| Voice Cloning | Explores AI-based voice generation and voice cloning | Python, AI Models |

---

# 📂 Projects

## 1. Image Enhancement and Text Extraction

**Folder:** `Image_enhacenment`

### Overview

The Image Enhancement and Text Extraction project focuses on improving the quality of images and extracting readable text from them.

Images captured from cameras, scanned documents, or other sources may contain noise, blur, poor resolution, and other imperfections. This project applies image-processing techniques to improve image quality before performing Optical Character Recognition (OCR).

### Key Features

- **Image Enhancement:** Improves the visual quality of input images.
- **Image Upscaling:** Increases image dimensions to improve readability.
- **Deblurring:** Applies processing techniques to improve the appearance of blurred images.
- **Padding:** Adds appropriate image borders to support processing.
- **Line Enhancement:** Improves text-line visibility.
- **Text Extraction:** Uses EasyOCR to identify and extract text from processed images.
- **Text Output:** Saves extracted text into a separate `.txt` file.

### Technologies Used

- Python
- OpenCV
- NumPy
- EasyOCR

### How It Works

1. The user provides an input image.
2. The application loads the image using OpenCV.
3. Image preprocessing techniques are applied.
4. The image is enhanced and prepared for OCR.
5. EasyOCR identifies and extracts text.
6. The enhanced image and extracted text are saved as output files.

### Execution

```bash
cd Image_enhacenment

python enhence_and_text.py
```

### Output Files

- `enhanced.jpg` – Enhanced image.
- `extracted_text.txt` – Extracted textual content.

**Real-world Applications:**
- Digitization of scanned documents.
- Text extraction from photographs.
- Improving readability of low-quality images.
- Processing printed documents and image-based text.

---

## 2. Audio Analyzer

**Folder:** `audio_analyzer`

### Overview

The Audio Analyzer is a Python-based application designed to analyze digital audio files and extract useful audio information.

It focuses on understanding the technical properties of audio files and processing audio information using multimedia tools.

### Key Features

- Audio file loading and processing.
- Audio format identification.
- Audio duration analysis.
- Audio properties inspection.
- Processing audio files using multimedia utilities.
- Extracting available technical information from audio files.

### Technologies Used

- Python
- FFmpeg
- FFprobe
- Audio Processing Libraries

### How It Works

1. The application accepts an audio file as input.
2. The audio file is processed using Python.
3. FFmpeg and FFprobe are used for multimedia inspection.
4. Relevant audio properties and information are extracted.
5. The application displays the analysis results.

### Execution

```bash
cd audio_analyzer

python audio_analyzer.py
```

The application uses `input.mp3` as its default input file. You can also provide an audio file path if supported by the script.

### Prerequisites

FFmpeg and FFprobe must be installed and accessible through the system PATH.

Verify installation:

```bash
ffmpeg -version
ffprobe -version
```

**Real-world Applications:**
- Audio file inspection.
- Multimedia format analysis.
- Digital audio processing.
- Understanding audio properties and metadata.

---

## 3. Image Analyzer

**Folder:** `image_analyzer`

### Overview

The Image Analyzer focuses on analyzing digital images and understanding their properties through image-processing techniques.

It demonstrates how Python can be used to load, process, and inspect digital images.

### Key Features

- Image loading and processing.
- Image property inspection.
- Image analysis using Python libraries.
- Processing digital image inputs.
- Displaying analysis results.

### Technologies Used

- Python
- OpenCV
- NumPy
- Image Processing Libraries

### How It Works

1. The user provides an image as input.
2. The application loads the image.
3. Image-processing operations are performed.
4. Relevant image information is analyzed.
5. Results are displayed to the user.

### Execution

```bash
cd image_analyzer

python Image_Analyzer.py <image_path>
```

Replace `<image_path>` with the actual image location. Check the script's entry-point filename if it differs.

**Real-world Applications:**
- Digital image inspection.
- Image-processing applications.
- Computer vision systems.
- Image-based data analysis.

---

## 4. Video Analyzer

**Folder:** `video_analyzer`

### Overview

The Video Analyzer focuses on processing and analyzing digital video files.

Video is a multimedia format that combines a sequence of visual frames and, in many cases, audio streams. This project explores how video files can be processed and analyzed using programming and multimedia tools.

### Key Features

- Video file input and processing.
- Video stream inspection.
- Video analysis using Python.
- Processing multimedia content.
- Extracting useful information from video inputs.

### Technologies Used

- Python
- OpenCV
- FFmpeg
- Video Processing Libraries

### How It Works

1. The application accepts a video file.
2. The video is loaded for processing.
3. The application analyzes the video content.
4. Video-processing operations are performed.
5. Relevant results are displayed.

### Execution

Navigate to the project folder and run its main Python script:

```bash
cd video_analyzer

python <main_script>.py <video_path>
```

Replace the placeholders with the actual script name and video file path.

**Real-world Applications:**
- Video processing and inspection.
- Multimedia content analysis.
- Computer vision applications.
- Video-based information processing.

---

## 5. Voice Cloning

**Folder:** `voice_cloning`

### Overview

The Voice Cloning project explores the application of Artificial Intelligence and speech synthesis to generate artificial speech that resembles a reference voice.

Voice cloning uses AI-based models to learn characteristics of a voice and generate speech with similar vocal characteristics.

### Key Features

- AI-based speech generation.
- Reference voice processing.
- Voice cloning experimentation.
- Text-to-speech generation.
- Integration with pretrained voice-generation models.
- API-based model inference.

### Technologies Used

- Python
- Artificial Intelligence
- Speech Synthesis
- Hugging Face
- MegaTTS
- Gradio Client

### How It Works

1. A reference voice or supported input is provided.
2. The application processes the input using an AI-based voice model.
3. The model performs speech-generation inference.
4. Generated speech is returned as audio output.
5. The generated audio can be played or saved.

### Execution

Navigate to the voice cloning directory:

```bash
cd voice_cloning
```

Install the dependencies specified by the project:

```bash
pip install -r requirements.txt
```

Run the project's main application script according to its implementation.

**Real-world Applications:**
- AI-powered speech synthesis.
- Accessibility and assistive technologies.
- Voice-based applications.
- Speech-generation research.
- Multimedia content production.

**Note:** Voice cloning should only be performed using voices for which appropriate permission and consent have been obtained.

---

# 🛠️ Technologies Used

The repository combines several programming technologies and multimedia-processing tools.

| Technology | Purpose |
|---|---|
| Python | Primary programming language |
| OpenCV | Image and video processing |
| NumPy | Numerical and array operations |
| EasyOCR | Optical Character Recognition |
| FFmpeg | Multimedia processing |
| FFprobe | Multimedia information inspection |
| Hugging Face | AI model integration |
| MegaTTS | AI-based speech generation |
| Gradio Client | Communication with AI model interfaces |
| Git & GitHub | Version control and project hosting |

---

# 📁 Repository Structure

```text
IC-2k22-02-Abhay-Singh-Thakur-Multimedia/
│
├── Image_enhacenment/
│   ├── enhence_and_text.py
│   ├── input.jpg
│   ├── enhanced.jpg
│   └── extracted_text.txt
│
├── audio_analyzer/
│   ├── audio_analyzer.py
│   └── input.mp3
│
├── image_analyzer/
│   └── Image Analyzer source files
│
├── video_analyzer/
│   └── Video Analyzer source files
│
├── voice_cloning/
│   └── Voice Cloning source files
│
└── README.md
```

---

# ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/abhayy11/IC-2k22-02-Abhay-Singh-Thakur-Multimedia-.git
```

### 2. Navigate to the Repository

```bash
cd IC-2k22-02-Abhay-Singh-Thakur-Multimedia-
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Required Libraries

Install the dependencies required by the individual projects.

For example:

```bash
pip install numpy opencv-python easyocr
```

Additional dependencies such as FFmpeg, FFprobe, and AI model packages may be required depending on the project.

**Important:** Each project may have its own dependency requirements. Install the required packages before running that particular application.

---

# 🌍 Real-World Applications

These projects demonstrate multimedia computing concepts that are useful across multiple domains.

- **Document Processing:** Enhancing images and extracting textual information.
- **Digital Media Analysis:** Inspecting image, audio, and video content.
- **Computer Vision:** Processing visual information using programming techniques.
- **Artificial Intelligence:** Applying AI models to speech and voice generation.
- **Multimedia Systems:** Understanding how different media formats can be processed programmatically.

---

# 🎓 Learning Outcomes

Through these projects, the following concepts and practical skills are explored:

- Understanding digital multimedia formats.
- Applying image-processing techniques.
- Implementing Optical Character Recognition.
- Working with audio and video processing tools.
- Understanding multimedia file properties.
- Integrating external AI models and APIs.
- Using Python libraries for multimedia applications.
- Understanding practical applications of Artificial Intelligence in multimedia systems.

---

# 👨‍💻 Author

**Abhay Singh Thakur**

Multimedia Systems Project

GitHub: [abhayy11](https://github.com/abhayy11)

**Repository:** [IC-2k22-02-Abhay-Singh-Thakur-Multimedia-](https://github.com/abhayy11/IC-2k22-02-Abhay-Singh-Thakur-Multimedia-)

---

⭐ If you find this repository useful, consider giving it a star!


