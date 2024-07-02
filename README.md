# Automatic-Speech-Recoginition-ASR

Automatic speech recognition is the task of transcribing spoken words to text is framed as sequence to sequence task using the transformer arcitecture. Raw speech waveform/Mel spectrogram is treated as a sequence of continous numbers and tokenized text is treated as a sequence of tokens.

We will build an Arabic ASR model without the hassle of creating complex model classes using Hugging Face Transformers🤗. We will finetune a pre-trained model (Whisper) from huggingface transformers.

![image](https://github.com/SaadElDine/Automatic-Speech-Recoginition-ASR-/assets/113860522/e2f9241f-5543-434b-87e9-12c334bd1d08)


# The ASR task is in 3 steps:

1. Feature Extraction: Here we extract audio features depending on model used, Whisper uses mel-spectrogram as it's input so we'll extract mel spectrogram from the audio. We'll also tokenize input arabic characters.
2. Model training: We train the model
3. Output Tokenizer: we tokenize the model's output back to arabic characters.
