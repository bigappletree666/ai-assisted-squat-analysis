# AI-Assisted Squat Analysis Project

Version: v1
Created: 2026-05-18

---

# 1. Project Overview

## Project Vision

Build a low-cost AI-assisted movement analysis platform using:

- smartphone video
- computer vision
- pose estimation
- biomechanics logic

The initial MVP focuses on:

- side-view squat analysis

Future expansion may include:

- gait analysis
- jump landing analysis
- balance testing
- ACL return-to-sport
- neuro rehab
- tele-rehab monitoring

---

# 2. Problem Statement

Current movement assessment in PT / rehab / sports performance often relies on:

- visual observation
- subjective judgment
- manual recording
- inconsistent tracking

High-end biomechanics labs provide accurate assessment but are:

- expensive
- difficult to access
- not scalable for most clinics

This project aims to create:

a low-cost, scalable, objective movement analysis workflow.

---

# 3. Team

## 梁sir

Role:
- Engineering Lead
- Computer Vision Lead

Responsibilities:
- Python architecture
- OpenCV pipeline
- MediaPipe integration
- angle calculation implementation
- Streamlit app
- GitHub management
- data pipeline

---

## 王sir

Role:
- Biomechanics Lead
- Research & Validation Lead

Responsibilities:
- biomechanics research
- squat movement analysis
- angle interpretation
- feedback rules
- testing & validation
- clinical wording
- report logic

---

# 4. MVP Scope (Phase 1)

## Goal

Build a working side-view squat analysis prototype before August 2026.

---

## Input

User uploads:

- side-view squat video

---

## System Pipeline

video
↓
pose estimation
↓
landmark extraction
↓
angle calculation
↓
movement analysis
↓
report generation

---

## Output Metrics

- knee angle
- hip angle
- ankle angle
- trunk lean
- squat depth
- lowest squat position
- basic movement observations

---

## Example Output

Lowest squat depth: 78°

Knee angle at bottom: 76°
Hip angle at bottom: 65°
Ankle angle at bottom: 41°

Observations:
- mild forward trunk lean
- squat depth within selected movement criteria
- possible reduced ankle dorsiflexion pattern

---

# 5. Important Clinical Positioning

This project is:

- AI-assisted movement assessment
- objective movement analysis
- computer vision biomechanics tool
- clinical decision support tool

This project is NOT:

- medical diagnosis
- injury diagnosis
- replacement for professional assessment

---

# 6. Tech Stack

## Initial Stack

- Python
- OpenCV
- MediaPipe
- NumPy
- pandas
- matplotlib
- Streamlit

---

## Future Stack

- PyTorch
- TensorFlow
- FastAPI
- React
- PostgreSQL
- cloud deployment
- LLM integration

---

# 7. Pose Estimation

## Initial Model

MediaPipe Pose

Reason:
- lightweight
- fast
- easy to prototype
- sufficient for MVP

---

## Key Landmarks

- shoulder
- hip
- knee
- ankle
- foot/toe

---

# 8. Biomechanics Logic

## Knee Angle

Definition:
hip → knee → ankle

Purpose:
- squat depth
- ROM analysis

---

## Hip Angle

Definition:
shoulder → hip → knee

Purpose:
- hip hinge
- trunk strategy

---

## Ankle Angle

Definition:
knee → ankle → foot

Purpose:
- ankle dorsiflexion estimation

---

## Trunk Lean

Definition:
shoulder-hip line relative to vertical

Purpose:
- movement strategy
- compensation pattern

---

# 9. Phase 1 Features

## Required Features

- video upload
- pose extraction
- angle calculation
- lowest squat detection
- graph generation
- movement report

---

## Not Included in Phase 1

- front-view valgus analysis
- ML training
- diagnosis
- patient database
- telehealth dashboard
- individualized anthropometric recommendations

---

# 10. Future Development Ideas

## Phase 2

- asymmetry analysis
- rep counting
- tempo analysis
- front-view analysis
- valgus detection

---

## Phase 3

- machine learning classification
- movement quality prediction
- compensation detection
- fatigue analysis

---

## Phase 4

- patient tracking
- clinician dashboard
- remote rehab monitoring
- SOAP note generation

---

# 11. Anthropometrics Vision (Future)

Future idea:

estimate body proportions using:

- standing photo
- reported height
- segment estimation

Potential variables:
- tibia length
- femur length
- trunk ratio

Goal:
better contextualize squat mechanics across different body structures.

NOTE:
This is NOT included in MVP Phase 1.

---

# 12. Folder Structure

Suggested project structure:

AI-Squat-Analysis/
│
├── app/
├── src/
├── data/
│   ├── raw_videos/
│   ├── processed/
│   └── csv/
├── reports/
├── notebooks/
├── docs/
├── tests/
├── README.md
└── requirements.txt

---

# 13. Weekly Roadmap

## Week 1
- setup environment
- run MediaPipe
- extract landmarks

## Week 2
- angle calculation

## Week 3
- squat bottom detection

## Week 4
- full pipeline

## Week 5
- movement rules

## Week 6
- Streamlit app

## Week 7
- report generation

## Week 8
- testing

## Week 9
- algorithm refinement

## Week 10
- demo build

## Week 11
- final polish

---

# 14. Current Development Status

## Current Phase

Phase 1 — Functional Prototype

---

## Current Progress

- project planning completed
- roadmap drafted
- MVP scope defined

---

# 15. Research Topics

Topics to review:

- squat biomechanics
- trunk lean
- ankle dorsiflexion
- tibia inclination
- squat depth
- hip-dominant vs knee-dominant squat
- body proportions and squat mechanics
- pose estimation reliability
- computer vision in rehab

---

# 16. Key Principles

The project focus is NOT:

"building the strongest AI"

The project focus IS:

AI + biomechanics + usable rehab workflow

Core value:
objective, scalable movement analysis.

---

# 17. Long-Term Vision

Build:

"a smartphone-based low-cost biomechanics lab"

Potential users:
- PT clinics
- rehab centers
- sports performance
- coaches
- athletes
- telehealth
- remote monitoring

---
