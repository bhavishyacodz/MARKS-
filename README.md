# Prepwise — JEE Main PYQ Practice

A mobile-friendly static JEE Main practice app hosted with GitHub Pages.

## Project structure

```text
MARKS-/
├── index.html              # App layout and practice logic
├── css/
│   └── style.css           # Responsive UI and component styles
├── data/
│   └── jee-main-2025.js    # Verified, paraphrased PYQs and worked solutions
└── README.md               # Project notes
```

## Current question set

- Current bank: 24 questions total — 12 sourced, paraphrased JEE Main 2025 PYQs (02 April, Shift 2) and 12 clearly labeled demo questions used to test the interface and practice features.
- Sourced PYQ batch: Physics 3, Chemistry 3, Mathematics 6. Demo set: 4 questions per subject.
- Demo questions are explicitly marked “Not an official PYQ”; do not treat them as previous-year questions.
- Sourced PYQ answers include NTA final-answer-key references. Every question includes options, concept, worked steps, and a final answer.
- Questions sort newest year/date/shift first. Use the “Demo set” year filter to test demo questions without mixing them with sourced PYQs.

## Run and deploy

This is a static site. GitHub Pages serves `index.html` and its relative CSS/data files directly. Keep these paths intact when editing. Publishing can take several minutes after a commit.

## Add more PYQs

Add question objects to `window.PYQ_QUESTIONS` in `data/jee-main-2025.js`. Use unique IDs and include subject, chapter, options, zero-based answer index, explanation steps, final answer, exam/session type, and source IDs. Verify each answer against the official final answer key before labeling it verified.

## Progress storage

Practice attempts and bookmarks are stored in browser localStorage under `prepwise_jee_starter_v1`. On load, progress linked to removed question IDs is discarded so the app statistics match the current question set.
