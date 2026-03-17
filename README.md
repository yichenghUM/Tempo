# Tempo
Tempo is an AI-powered academic planning assistant that integrates Canvas and Google Calendar to turn assignments, lecture materials, and deadlines into personalized study plans using RAG-based resource matching and AI task estimation.

## Setup

1. Install dependencies:
   pip install -r requirements.txt

2. Get a free Gemini API key:
   https://aistudio.google.com/apikey

3. Set your API key:
   # Mac/Linux
   export GEMINI_API_KEY=your_key_here

   # Windows (PowerShell)
   $env:GEMINI_API_KEY="your_key_here"

   # Windows (CMD)
   set GEMINI_API_KEY=your_key_here

4. Run the server:
   python server.py

5. Open your browser to:
   http://localhost:5000

## How it works

1. Enter your uniqname and course (e.g. EECS 281)
2. Upload your assignment PDF (and optionally your notes)
3. Gemini analyzes the assignment content + historical timing data
   from other students to estimate how long it should take
4. Start the timer and work — it tracks time vs. estimate in real time
5. When done, hit Done — your session is saved and improves future estimates
