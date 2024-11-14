# WELLNESS_AI

🌟 Wellness & Mental Health Assistant
Overview
The Wellness & Mental Health Assistant is an interactive mental wellness tracking and management tool built using Gradio and various machine learning libraries. It provides a personalized interface for users to track their mood, set goals, establish healthy habits, journal their thoughts, and receive recommendations based on their emotional patterns. It also includes mindfulness, wellness tips, and daily inspirational quotes for ongoing mental support.

Key Features
Mood Tracking: Users can rate their mood daily, select emotions they are experiencing, and add notes. This information generates insights based on recent mood history.
Journaling: Provides journaling options, allowing users to categorize entries (e.g., Gratitude, Reflection) and track thoughts or goals.
Goal Setting & Habit Tracking: Users can set personal wellness goals with target dates and create habit routines with tracking capabilities.
Wellness Report: Offers a comprehensive wellness report summarizing mood insights, goals, habits, and daily recommendations.
Mindfulness & Wellness Tips: Contains built-in resources like meditation guides, exercise routines, and wellness tips to support mental and physical health.
Daily Quotes: Displays motivational and mental health-related quotes to inspire users.
Components & Architecture
WellnessAI Class
The core of the application, WellnessAI, handles the following functions:

Initialization: Loads necessary resources, NLP models, and stored user data.
Mood Tracking & Insights: Records mood scores and emotions and provides insights such as mood trends, average score, and recent emotional patterns.
Journal Entries: Supports various types of journal entries and allows users to tag entries for better organization.
Goals & Habits: Manages user-defined goals with target dates and tracks habits, storing details like streak and frequency.
Wellness Recommendations: Analyzes user data to offer personalized wellness tips based on mood and activity history.
Wellness Report Generation: Compiles a summary report of mood insights, goals, habits, and recommendations for an easy overview.
WellnessUI Class
The WellnessUI class creates an interactive Gradio interface with multiple tabs:

Mood Tracker Tab: Collects mood scores, emotions, and notes, providing insights into recent mood history.
Journal Tab: Allows entry of journal content with tags, offering options for different entry types (Gratitude, Reflection, etc.).
Goals & Habits Tab: Includes options for setting wellness goals and tracking habits with specified frequencies.
Wellness Report Tab: Generates a wellness report based on stored data and displays insights, goals, habits, and recommendations.
ML Models and Resources
NLP Models: Uses NLP models from Hugging Face (e.g., DialoGPT for therapy-style interaction and distilroberta for emotion classification).
Sentiment Analysis: Uses nltk’s VADER Sentiment Analyzer for basic sentiment analysis on journal entries.
Wellness Tips and Exercises: Provides pre-defined wellness activities, coping strategies, meditation guides, and exercise routines for users to engage with.
Installation & Requirements
To run this assistant, ensure the following libraries are installed:

Python 3.7+
Gradio: pip install gradio
Pandas: pip install pandas
TensorFlow: pip install tensorflow
Transformers: pip install transformers
Torch: pip install torch
OpenCV: pip install opencv-python
MediaPipe: pip install mediapipe
NLTK: pip install nltk
Plotly: pip install plotly
Pillow: pip install pillow
To download NLTK data:

python
Copy code
import nltk
nltk.download('vader_lexicon')
nltk.download('punkt')
nltk.download('stopwords')
Usage
Run the Interface: Execute the script by running python wellness_assistant.py. This will launch the Gradio app locally with a shareable link if specified.
Access Tabs: Explore each tab (Mood Tracker, Journal, Goals & Habits, and Wellness Report) to use the different features.
Interact and Track Progress: Track mood, create journal entries, set goals, manage habits, and generate wellness reports to stay updated on mental health progress.
Data Storage
User data is saved locally in user_data.json. This file stores information on mood history, journal entries, goals, and habits, allowing continuity between sessions.

Project Structure
The script follows a class-based structure:

WellnessAI: Handles backend logic, data management, and ML model usage.
WellnessUI: Manages the Gradio interface and connects user inputs to backend functions.
Future Improvements
Advanced Analytics: Deeper mood analysis using time-series data for improved trend tracking.
Social Support: Add community-driven or social support options.
Gamification: Add rewards for habit streaks or completed goals to encourage engagement.
Credits
Built with the support of open-source ML and NLP tools: Hugging Face Transformers, NLTK, Gradio, and various mental health resources.








