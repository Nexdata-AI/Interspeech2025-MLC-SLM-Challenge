# Interspeech2025-MLC-SLM-Challenge
The Interspeech 2025 Multilingual Conversational Speech LLM (MLC-SLM) Challenge

## Motivation
Large Language Models (LLMs) have demonstrated remarkable capabilities across a variety of downstream tasks, serving as powerful foundation models for language understanding and generation. Recently, there has been significant interest in applying LLMs to speech and audio processing tasks, including Automatic Speech Recognition (ASR), Audio Captioning, and emerging areas such as Spoken Dialogue Models. 

However, the development of robust LLM-based Spoken Dialogue Models relies heavily on real-world conversational speech data, which encapsulates the complexity of human communication, including natural pauses, interruptions, speaker overlaps, and diverse conversational styles. The scarcity of such data, especially in multilingual contexts, poses a significant challenge to advancing the field. 

The importance of real-world conversational speech extends beyond technological advancement—it is essential for building AI systems that can understand and respond naturally in multilingual, dynamic, and context-rich environments. This is especially crucial for next-generation human-AI interaction systems, where spoken dialogue serves as a primary mode of communication.

Thus, this workshop aims to bridge the gap by hosting the challenge of building multilingual conversational speech language models (MLC-SLM) together with the release of a real-world multilingual conversational speech dataset. 

## Task Setting and Evaluation
The challenge consists of two tasks, both of which require participants to explore the development of speech language models (SLMs):

### Task 1: Multilingual Conversational Speech Recognition

Objective: Develop a multilingual LLM-based ASR model.

Participants will be provided with oracle segmentation and speaker labels for each conversation. 

This task focuses on optimizing recognition accuracy in a multilingual conversation setting.

### Task 2: Multilingual Conversational Speech Diarization and Recognition

Objective: Develop a system for both speaker diarization (identifying who is speaking when), and recognition (transcribing speech to text). 

No prior or oracle information will be provided during evaluation (e.g., no pre-segmented utterances or speaker labels).

Both pipeline-based and end-to-end systems are encouraged, providing flexibility in system design and implementation.

For Task I, system performance will be evaluated using Word Error Rate (WER) or Character Error Rate (CER) across different languages.

For Task II, performance will be assessed based on the Diarization Error Rate (DER) and the concatenated minimum permutation WER or CER, referred to as cpWER or cpCER. The DER is employed to determine the best speaker ID permutation between oracle annotation and diarization results. Then, the recognition results and references belonging to the same speaker within a recording will be concatenated to calculate the cpWER or cpCER. All submissions will be ranked according the cpWER or cpCER.

## Important Dates
March 10, 2025: Registration opens

March 15, 2025: Training data release

March 20, 2025: Development set and baseline system release

May 15, 2025: Evaluation set release and leaderboard open

May 30, 2025: Leaderboard freeze and paper submission portal opens (CMT system)

June 15, 2025: Paper submission deadline

July 1, 2025: Notification of acceptance

August 18, 2025: Workshop date

## Dataset Description
### Training set
The training set (Train) comprises approximately 11 languages: English (en), French (fr), German (de), Italian (it), Portuguese (pt), Spanish (es), Japanese (jp), Korean (ko), Russian (ru), Thai (th), Vietnamese (vi).
Each recording consists of two-speaker conversational speech on randomly assigned topics. 

Conversations are natural and fluent, with speakers engaging in meaningful dialogues on each topic. 

Recorded in quiet indoor environments using devices such as iPhones. 

Each recording will provide the oracle segmentation and speaker label for the development of speech recognition and speaker diarization systems.

Both Task I and Task II share the same training set.

The English dataset comprises approximately 500 hours of recordings from various regions, including British, American, Australian, Indian, and Philippine English. Other languages contribute around 100 hours each, resulting in a total of approximately 1500 hours of multilingual conversational speech data.

This dataset is designed to provide a rich resource for training and evaluating multilingual conversational speech language models (MLC-SLM), addressing the challenges of linguistic diversity, speaker variability, and contextual understanding.

### Development set
The development set (Dev) has the same setting as the training set but contains approximately 4 hours of recordings for each language. Both Task I and Task II share the same development set.

### Evaluation set
Different evaluation sets are employed for each task, designated as Eval_1 and Eval_2. Specifically, Eval_1 includes oracle timestamps and speaker labels, which are evaluated using WER/CER. Eval_2 does not provide timestamps or speaker labels, necessitating a speaker diarization (SD) system to segment the longer recordings before recognition.

Participants can access the dataset by signing the Data use agreement and submitting to the registration form. After submission, the data download link will be sent to your email.

## Rules
All participants must adhere to the following rules to be eligible for the challenge.   
Use of External Resource: For both Track I and Track II, the use of external datasets and pre-trained models (including speech foundation models and LLMs) is permitted. All external resources utilized must be freely accessible to all research groups and should be clearly indicated in the final system report.   

Data augmentation: Data augmentation is allowed on the released training set and may include, but is not limited to, the addition of noise or reverberation, speed perturbation, and tone modification.  

Prohibition of Evaluation Sets Usage: The use of evaluation sets in any form of non-compliance is strictly prohibited. This includes, but is not limited to, using evaluation sets for fine-tuning or training the model.  

Multi-System Fusion: Participants are NOT allowed to employ system fusion in either Task I and Task II. Submitted results must be derived from a single model rather than through result fusion.   

Submission Requirement：All participations are required to submit their system. The submission may include final results, models and a Docker that can directly perform inference to obtain the final results, etc. Detailed submission instructions will be provided following the release of the baseline implementation. Please note that we will publicly disclose the name of teams and their affiliated institutions that confirmed participation but did not submit any files. 

Organizer's Interpretation: The organizers reserve the right to make the final interpretation of these rules. In special circumstances, the organizers will coordinate the interpretation as needed.

## Other Topics
In addition to challenge system descriptions, participants are encouraged to submit research papers that showcase innovative findings, practical case studies, and forward-looking ideas. Topics of interest include, but are not limited to:   

Novel Architectures and Algorithms: Development of new architectures and algorithms for training SLMs.   

Audio Data Processing Pipelines: Innovative pipelines for processing raw audio data that facilitate the collection of diverse internet data for training SLMs. 

Natural and Emotionally Rich Speech Generation: Algorithms designed to generate more natural and emotionally expressive conversational speech for dialogue systems.   

Leveraging Multi-Turn Conversational History: Approaches that utilize multi-turn conversational history to enhance recognition and diarization results.  

Evaluation Techniques and Benchmarks: Innovative evaluation techniques or benchmarks specifically tailored for assessing SLMs.   

New Datasets: Creation of new datasets, both real and synthetic, for training speech and audio language models.   

## Data Access and Usage
Registered participants will be given access to the training and testing datasets. They must sign a data use agreement (see below), agree to confidentiality and comply with the data protection agreement. The datasets will only be used for the purpose of the workshop challenge, and redistribution or any other use is strictly prohibited. It is the responsibility of the participant to protect the data from unauthorized access.

[Data use agreement](https://www.nexdata.ai/nexdata/static/file/doc/Data-use-agreement-nexdata.docx)

## Registration
To participate, registration is required. Please upload signed Data use agreement and complete the [registration form](https://docs.google.com/forms/d/e/1FAIpQLSftZCRQQWvO5NZd-bPo1VT2Xsaieu_ZYCklw6MhW6LqjWnuYQ/viewform?usp=send_form) The challenge begins on March 10, 2025.

For any other information about registration, please send Email to: mlc-slmw@nexdata.ai

More details：https://www.nexdata.ai/competition/mlc-slm

## Baseline System
Will be released soon.

## Leaderboard Submission
Will be released soon.

## Prize Pool
Prizes for Top-Ranking Teams in this Competition(each task):
1st Place:$5,000   
2nd Place:$3,000   
3rd Place:$2,000   

## Organizers
Lei Xie, Professor, Northwestern Polytechnical University (China)   
Shinji Watanabe, Associate Professor, Carnegie Mellon University (USA)   
Eng Siong Chng, Associate Professor, Nanyang Technological University (Singapore)   
Junlan Feng, IEEE Fellow & Chief Scientist, China Mobile (China)   
Khalid Choukri, Secretary General, European Language Resources Association (France)   
Qiangze Feng, Co-founder & Data Scientist, Nexdata (USA)   
Daliang Wang, Data Scientist, Nexdata (USA)   
Hexin Liu, Postdoctoral Researcher, Nanyang Technological University (Singapore)   
Pengcheng Guo, PhD Student, Northwestern Polytechnical University (China)   
Bingshen Mu, PhD Student, Northwestern Polytechnical University (China)   
Zhaokai Sun, Master Student, Northwestern Polytechnical University (China)   
