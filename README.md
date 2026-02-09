*📰 Fake News Detector for Students*
A machine learning-powered web application designed to help students and researchers identify potentially unreliable news articles. This tool analyzes text for credibility and provides a concise summary of the content using state-of-the-art Natural Language Processing (NLP) models.

🚀 Features
Credibility Analysis: Classifies news articles as "REAL" or "FAKE" using a fine-tuned BERT model.

Confidence Score: Displays a percentage score indicating the model's certainty in its prediction.

AI Summarization: Generates a short, digestible summary of long articles using the BART model (facebook/bart-large-cnn).

Fact-Check Verification: Provides a direct link to search the topic on Google News for cross-referencing.

Session History: Keeps a temporary log of analyzed articles during your session.

Export Data: Download your analysis history as a .csv file for research or assignments.

Custom UI: Features a modern "Dark Navy" interface optimized for readability.

🛠️ Tech Stack
Frontend: Streamlit (Python web framework)

Machine Learning: Hugging Face Transformers

Classifier: jy46604790/Fake-News-Bert-Detect

Summarizer: facebook/bart-large-cnn

Backend/Tunneling: PyNgrok (To host the app from Google Colab)

Libraries: PyTorch, Pandas, Numpy

📦 How to Run (Google Colab)
Get an Ngrok Token:

Sign up for free at ngrok.com.

Copy your Authtoken from the dashboard.

Configure the Code:

Paste your Ngrok token into the script where indicated:

Python
conf.get_default().auth_token = "YOUR_TOKEN_HERE"
Execute:

Run the script cell in Google Colab.

Wait for the dependencies and models to download.

Click the public URL generated at the bottom (e.g., https://xyz.ngrok-free.app).

📝 Usage Guide
Paste Text: Copy the content of a news article, blog post, or social media message into the main text box.

Adjust Settings: Use the sidebar to set the maximum length for the summary.

Analyze: Click the "🔍 Analyze" button.

Review Results:

Check the Verdict (Real vs. Fake) and the Confidence %.

Read the AI-generated Summary.

Use the "Verify on Google News" link to see if major outlets are reporting the same story.

⚠️ Disclaimer
This tool uses AI models trained on specific datasets to predict credibility. It is not infallible.

False Positives/Negatives: The model may occasionally misclassify satire, opinion pieces, or very recent events not in its training data.

Educational Use Only: Always verify critical information with multiple trusted sources.

🤝 Credits
Developer: Keerthikeshan K

Frameworks: Streamlit, Hugging Face

Models: BERT (Google), BART (Facebook)

© 2026 Fake News Detector Project
