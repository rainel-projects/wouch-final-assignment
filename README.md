
<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/a59ea1e2-c049-4fb1-89a0-8ddc1f8f90df" />


Emotional Safety Engine — Weighted Psychology Model

Live Demo → https://rainel-projects.github.io/wouch-final-assignment/

GitHub Repo → https://github.com/rainel-projects/wouch-final-assignment.git

🌿 Overview

The Emotional Safety Engine is an interactive emotional-check-in tool designed to help users explore their relationship patterns with compassion.
It’s not just a form — it is a mini emotional intelligence system that responds gently, adapts to vulnerability, and calculates a personalized emotional safety score.

This project was built for a technical + psychological challenge with a focus on:

User empathy

Conditional emotional logic

Soft + safe UI/UX

Clean JavaScript architecture

Weighted scoring based on psychology markers

🧠 How the Logic Works

The engine collects three core answers:

Emotional response to delayed replies

Relationship pattern (staying longer than they should)

Biggest dating fear (free-text)

Then it runs through:

1️⃣ Weighted Emotional Logic

Each emotion (Anxious / Angry / Indifferent / Sad / Confused) has a carefully chosen psychological weight.

Example:

Anxious = −30

Angry = −15

Indifferent = −5

Sad = −20

Confused = −12

These weights reduce the baseline score because each emotion represents different levels of emotional activation or distress.

2️⃣ Follow-Up Sensitivity Analysis

Based on follow-up answers (Yes/No/Withdraw/Confront/Both), the score adjusts further.

Example:

“Yes, I worry what others think” → −10

“No” → +8

Withdraw → −8

Confront → −3

3️⃣ Text Emotion + Clarity Analysis

The fear text is processed for emotional signals:

Warm words → boosts tone

Harsh words → reduces tone

Fear words → reduces tone

Low-clarity words (“idk”, “maybe”) → reduces clarity

Confident phrases → boosts confidence

Hesitant phrases → reduces confidence

Vulnerability markers → increase vulnerability score

This becomes a small natural-language scoring engine inside your form.

4️⃣ Final Emotional Safety Score

All factors are combined into a 0–100 score with 3 emotional ranges:

75–100 → Healthy emotional awareness

40–74 → Carrying emotional weight

0–39 → Needs emotional safety support

Each score triggers a different, compassionate message.

✨ ✨ New Features I Added (Beyond Requirements)
1. 🌡️ Real-Time Sub-Scores (NEW)

I added three new sub-metrics not required in the original problem:

Tone Score (emotional warmth vs emotional distress)

Confidence Score (certainty vs hesitation in language)

Clarity Score (linguistic clarity + emotional coherence)

These make the tool feel deeper, more meaningful, and more emotionally aware.

2. 🔍 Micro-Emoji + Word-Level Emotion Detection (NEW)

The engine scans text for:

warm emotional words

harsh emotional words

fear markers

clarity markers

confident vs hesitant phrasing

vulnerability indicators

This is a tiny psychological NLP engine, built manually with weighted scoring — no libraries.

3. 🐬 Dolphin Completion Affirmation (NEW)

When the user finishes the form:

progress bar animates to 100%

replaces % with 🐬 100%

creates a calming emotional reward moment

This small detail reduces anxiety and reinforces safety.

4. ❤️ Safe, Soft, Non-Clinical UI (NEW)

I created a UI inspired by:

Apple Health calm vibes

oceanic gradient (therapy blue)

glass-blur panels

floating animation

soft typography

breathing-space layout

This ensures the user never feels judged or overwhelmed.

📐 Tech Stack

Pure HTML / CSS / JavaScript

No frameworks — built from scratch for clarity and transparency

Deployed on GitHub Pages

🧭 Folder Structure
.
├── index.html
└── .github/workflows/main.yml

🚀 Deployment (GitHub Pages)

The app is built automatically using a GitHub Actions workflow:

name: Deploy

on:
  push:
    branches: ["main"]

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/upload-pages-artifact@v3
        with:
          path: .
      - uses: actions/deploy-pages@v4


Result → https://rainel-projects.github.io/wouch-final-assignment/

🎨 Design Choices (Short and Clear)

Why I built it this way:

I wanted the experience to feel emotionally safe and not like a clinical form.

Layout is balanced: left = vulnerability questions, right = supportive guidance.

Colors, spacing, and micro-interactions were chosen to lower emotional activation.

What I prioritized:

Clear emotional logic

Human tone

Soft UI

No confusion or cognitive load

Instant progress feedback

Kind, validating messages

What I’d improve with more time:

Add anonymous save & resume

Add dark/light theme

Improve NLP with sentiment scoring

Add guided resources tailored to answers

Voice-over calming assistant mode

🧡 Created with care by Veda

This project is built with empathy, psychology insight, and clean logical structure — designed to make someone who has been hurt in dating feel understood and safe.
