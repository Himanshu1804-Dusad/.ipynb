# .ipynb
Assignment: Call Quality Analyzer
##***
I used OpenAI Whisper for transcription since it handles noisy audio well and runs on Colab’s free GPU. The audio is downloaded and converted into text. Speaker diarization is simulated using silence-based segmentation, alternating between sales rep and customer. From the transcript, I computed:

Talk-time ratio by word distribution.

Number of questions by detecting ? in text.

Longest monologue using silence splits.

Sentiment analysis with HuggingFace transformers.

Actionable insight rule-based on balance of talk-time and questions.

The system works under 30s on Colab (small Whisper model). Bonus attempt: sales rep vs customer is approximated by alternating speaker turns.

**##
