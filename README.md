# Interspeech2025-MLC-SLM-Challenge
The Interspeech 2025 Multilingual Conversational Speech LLM (MLC-SLM) Challenge

## Motivation
Large Language Models (LLMs) have demonstrated remarkable capabilities in a wide range of downstream tasks, serving as powerful foundation models for language understanding and generation. Furthermore, there has been significant attention on utilizing LLMs in speech and audio processing tasks such as Automatic Speech Recognition (ASR), Audio Captioning, and emerging areas like Spoken Dialogue Models.

However, real-world conversational speech data is critical for the development of robust LLM-based Spoken Dialogue Models, as it encapsulates the complexity of human communication, including natural pauses, interruptions, speaker overlaps, and diverse conversational styles. The limited availability of such data, especially in multilingual settings, poses a significant challenge to advancing the field.

The importance of real-world conversational speech extends beyond technological advancement—it is essential for building AI systems that can understand and respond naturally in multilingual, dynamic, and context-rich environments. This is especially crucial for next-generation human-AI interaction systems, where spoken dialogue serves as a primary mode of communication.

Thus, this workshop aims to bridge the gap by hosting the challenge of building multilingual conversational speech language models together with the release of a real-world multilingual conversational speech dataset.

## Task Setting
The event consists of two tasks, both of which require participants to explore the development of speech language model:

### Task 1: Multilingual Conversational Speech Recognition

Participants will be provided with oracle segmentation for each conversation.

Objective: Develop a multilingual LLM based ASR model

This task focuses on optimizing transcription accuracy in a multilingual setting.

### Task 2: Multilingual Conversational Speech Diarization and Recognition

No prior or oracle information will be provided during evaluation (e.g., no pre-segmented utterances or speaker labels).

Objective: Develop a system for both speaker diarization (identifying who is speaking when), and recognition (transcribing speech to text).

Both pipeline-based and end-to-end systems are encouraged, providing flexibility in system design and implementation.
