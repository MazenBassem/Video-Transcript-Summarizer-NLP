# Video Transcript Summarizer (NLP)

A lightweight NLP workflow for summarizing long-form video transcripts using Python and Jupyter.

This repository contains the notebook `text-summarizer.ipynb`, which demonstrates how to preprocess transcript text and generate concise summaries.

## 📌 Overview

The goal of this project is to reduce lengthy transcript content into short, readable summaries while preserving core meaning.

Typical use cases:
- Summarizing educational lecture transcripts
- Creating quick previews for long videos
- Extracting key points from interviews, talks, and podcasts

## 🧠 Notebook Included

- `text-summarizer.ipynb` — End-to-end summarization workflow in Jupyter

## ⚙️ Requirements

Use Python 3.10+ (3.12 also works) and install common NLP dependencies.

Example:

```bash
pip install -U jupyter nltk spacy scikit-learn pandas numpy matplotlib
```

> If your notebook uses additional libraries, install those as needed.

## 🎥 Choose the Video to Summarize

In the notebook, paste the link of the video you want to summarize (for example, a YouTube link), then run the cells in order.

Example:

```python
video_url = "https://www.youtube.com/watch?v=YOUR_VIDEO_ID"
```

## 🔑 Gemini API Key (Quick Setup)

You need a Gemini API key to run the summarization parts.

1. Open **Google AI Studio**: https://aistudio.google.com/
2. Click **Get API key**
3. Create and copy your key

### Option 1: Kaggle / Colab (Recommended for Notebooks)

- **Kaggle**: add your key using **Add-ons / Secrets** and read it in the notebook.
- **Google Colab**: use Colab secrets (or equivalent secure key storage) and load it in your notebook.

### Option 2: Terminal Environment Variable

#### Bash (Linux/macOS)

```bash
export GEMINI_API_KEY="your_api_key_here"
```

#### Windows CMD

```cmd
set GEMINI_API_KEY=your_api_key_here
```

#### Windows PowerShell (current session)

```powershell
$env:GEMINI_API_KEY="your_api_key_here"
```

#### Windows PowerShell (persist for future sessions)

```powershell
setx GEMINI_API_KEY "your_api_key_here"
```

> After `setx`, restart your terminal/IDE so the variable is available.

### Verify the key is set

#### Bash

```bash
echo $GEMINI_API_KEY
```

#### Windows CMD

```cmd
echo %GEMINI_API_KEY%
```

#### PowerShell

```powershell
echo $env:GEMINI_API_KEY
```

> Keep your API key private. Never hardcode it in public notebooks or commit it to GitHub.

## 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/MazenBassem/Video-Transcript-Summarizer-NLP.git
cd Video-Transcript-Summarizer-NLP
```

2. Launch Jupyter:

```bash
jupyter notebook
```

3. Open `text-summarizer.ipynb` and run the cells in order.

## 🧪 Typical Workflow in the Notebook

1. Load transcript text data
2. Clean and preprocess text (normalization, tokenization, stopword removal, etc.)
3. Apply summarization strategy/model
4. Review and compare generated summaries

## 📂 Project Structure

```text
Video-Transcript-Summarizer-NLP/
├── README.md
└── text-summarizer.ipynb
```

## ✅ Output

The notebook produces condensed summaries from raw transcript text, helping users quickly understand long video content.

## 🔮 Possible Improvements

- Add extractive vs. abstractive summary comparison
- Add ROUGE/BLEU evaluation metrics
- Add a simple CLI or Streamlit UI
- Support direct YouTube transcript ingestion

## 🤝 Contributing

Contributions are welcome. Feel free to open an issue or submit a pull request.

## 📜 License

Add a license file (e.g., MIT) if you plan to distribute this project publicly.
