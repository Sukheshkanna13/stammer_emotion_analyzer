# stammer_emotion_analyzer
This project is a hybrid deep learning-based system that identifies emotional states from speech recordings of individuals with stammering. By leveraging both spectrogram image analysis and speech transcription, the model effectively accounts for disfluencies like repetitions, prolongations, and blocks. The system generates stammering scores alongside emotional classifications, offering insights into the emotional patterns and fluency levels of the speaker.

🧠 Technologies & Process Flow

Audio Preprocessing

Format conversion from .mp3 to .wav

Noise removal, volume normalization, and sample rate standardization using Librosa

Transcription & Metadata Extraction

Speech-to-text using models like Google Speech Recognition or OpenAI Whisper

Stammering detection by counting disfluencies

Sentiment analysis on transcribed text using VADER/TextBlob

Feature Extraction

Mel-Spectrogram and MFCC features derived using Librosa

Spectrograms used as input for CNN-based emotion classification

Emotion Classification

Hybrid CNN-LSTM architecture for spatial and temporal feature learning

Fine-tuned YAMNet model as an alternative

Trained to detect 8 emotions: neutral, calm, happy, sad, angry, fearful, disgust, surprised

Model Evaluation

Metrics: Accuracy, Precision, Recall, F1-Score

Data augmentation techniques: noise addition, pitch shift, and time-stretching

Output

For each audio sample:

Transcribed text

Detected emotion

Stutter count

Sentiment score

Stammering score
