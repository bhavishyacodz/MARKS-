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

- Only verified JEE Main PYQs are shown; starter/sample questions have been removed.
- Current batch: Physics, Chemistry and Mathematics, 02 April 2025, Shift 2 (12 questions total: 3 Physics, 3 Chemistry and 6 Mathematics).
- Answers were checked against the NTA final answer key. Questions are paraphrased for practice.
- Each question includes options, concept, worked steps, final answer, and NTA question/option IDs.

## Run and deploy

This is a static site. GitHub Pages serves `index.html` and its relative CSS/data files directly. Keep these paths intact when editing. Publishing can take several minutes after a commit.

## Add more PYQs

Add question objects to `window.PYQ_QUESTIONS` in `data/jee-main-2025.js`. Use unique IDs and include subject, chapter, options, zero-based answer index, explanation steps, final answer, exam/session type, and source IDs. Verify each answer against the official final answer key before labeling it verified.

## Progress storage

Practice attempts and bookmarks are stored in browser localStorage under `prepwise_jee_starter_v1`. On load, progress linked to removed question IDs is discarded so the app statistics match the current question set.
