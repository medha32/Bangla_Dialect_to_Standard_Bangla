# Bangla_Dialect_to_Standard_Bangla

# 🗣️ Bangla Dialect → Standard Bangla Transformation
This project focuses on transforming Bangla dialect speech/text into Standard Bangla using transformer-based models. It was developed as part of Televerse 1.0 AI-Fication, where our team Neuralsight became a finalist for building a robust dialect-normalization system.

# 🚀 Project Overview

Bangla has many regional dialects that differ significantly from Standard Bangla, creating challenges for automatic speech/text understanding systems.
Our goal was to build an end-to-end model capable of converting dialect inputs into standardized Bangla, enabling:

✔ Better speech-to-text accuracy
✔ Improved NLP pipelines
✔ More accessible communication tools for diverse Bangladeshi dialects

We worked on both speech and text modalities and fine-tuned transformer-based architectures for optimal dialect → standard mapping.


# 🧠 Model Architecture

We used a combination of Wav2Vec2 (for speech) and Seq2Seq Transformers (for text), with fine-tuning tailored to dialect phonetics and vocabulary.

Speech Model

Architecture: Wav2Vec2 Base (pretrained on Bengali/Multilingual datasets)

Loss Function: CTC (Connectionist Temporal Classification)

Purpose: Align dialect speech to standardized text form

Optimizations:

Custom character vocabulary

Noise-augmented audio

Dialect-specific training samples

Text Model

Architecture: Seq2Seq Transformer (Encoder–Decoder)

Task: Dialect → Standard Bangla text rewriting

Techniques:

Token-level supervision

Beam search decoding

Domain-specific preprocessing


# ✨ Key Features

🔄 Dialect-to-Standard mapping for speech + text

🎙️ Fine-tuned Wav2Vec2 + CTC for speech normalization

📝 Fine-tuned Seq2Seq models for text rewriting

📈 Improved accuracy on dialectal variations


#Training Pipeline

Load & preprocess dialectal speech + text pairs

Train speech model with CTC for alignment

Fine-tune Seq2Seq model for text transformation

Evaluate dialect → standard accuracy

Run inference pipeline for validation



# 📌 Example Inference

| Dialect Input (Speech)      | Standard Bangla Output     |
|----------------------------------|-----------------------------|
| “তুমি কই যাইবা?”                | “তুমি কোথায় যাবে?”       |
| “এইডা কেডা করল?”               | “এটা কে করল?”             |
| “আমরা গইলাম বাজারে।”           | “আমরা বাজারে গেলাম।”      |



Members:
Utpal Barua
Nuzhat Tabassum



