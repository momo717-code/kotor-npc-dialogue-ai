AI NPC Dialogue System — KOTOR Bastila Shan
An AI-powered conversational system that generates in-character dialogue for Bastila Shan from Star Wars: Knights of the Old Republic, built iteratively from rule-based matching to generative AI with voice interaction.
Overview
This group project explores how AI can create believable NPC dialogue for video games. The system was developed through three progressive iterations, each adding complexity and capability, culminating in a voice-interactive conversational agent powered by DialoGPT and semantic similarity matching.
Development Iterations
Version 1 — Rule-Based CSV Matching

Pure Python logic with no AI involvement
Player input matched against existing KOTOR dialogue from a CSV dataset
Simple but limited — could only return pre-written lines

Version 2 — Generative AI with Ollama

Integrated Ollama for locally-hosted generative responses
Responses grounded in Bastila's character background and existing dialogue examples
Significant improvement in conversational flexibility

Version 3 — DialoGPT + Semantic Similarity + Voice

DialoGPT for generating contextual responses based on character profile and dialogue examples
Sentence-transformers for semantic similarity matching between player input and existing dialogue
Speech recognition (speech_recognition) for voice input
Text-to-speech (gTTS) for spoken NPC responses
Hugging Face amaydle/npc-dialogue dataset integrated for broader dialogue training

Tech Stack

Python — core language
Hugging Face Transformers — DialoGPT model for text generation
sentence-transformers — semantic similarity for dialogue matching
gTTS — Google Text-to-Speech for voice output
SpeechRecognition — voice input processing
pandas — dialogue dataset management
Ollama — local LLM integration (Version 2)

Project Structure
├── AIsolutionsCode.ipynb    # Full notebook with all three iterations
└── README.md
How to Run
bashpip install transformers torch sentence-transformers gTTS SpeechRecognition pandas datasets
Open AIsolutionsCode.ipynb in Google Colab or Jupyter and run the cells sequentially. Voice features require microphone access.
What I Learned

Iterative development from simple rule-based systems to generative AI demonstrates how each layer of complexity adds value
Semantic similarity matching bridges the gap between rigid scripted dialogue and fully generative responses
Voice integration adds a significant layer of immersion but introduces latency and accuracy challenges
Character consistency is one of the hardest problems in generative NPC dialogue

Academic Context
MSc AI for Software Development — AI Solutions module (group project), University of Dundee (2026).
