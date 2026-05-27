Overview: StudentBuddy is a cross‑platform (Android, iOS, Web) Flutter application that acts as a 24/7 personalized tutor and academic hub. It combines an AI Mentor chat (text + OCR image analysis), a distraction‑free Test Arena with anti‑cheat controls, adaptive roadmaps that track learning progress, and rich analytics (radar/line charts) to highlight strengths and weaknesses.
Users & Roles: Designed for Students, Admins, and SuperAdmins with role‑based UI and secure navigation. Admins can manage tests, configs, and view aggregated analytics.
Core Value: Replace fragmented study tools with a single, engaging app that blends generative AI help, automated assessment, and data‑driven guidance to improve study habits and outcomes.
Key Features:

AI Mentor Chat: Contextual help, problem explanations, and homework analysis using generative AI and OCR for images of handwritten work.
Test Arena: Timed, distraction‑minimized testing environment with anti‑cheat measures and immediate score breakdowns.
Analytics & Insights: Visual performance dashboards (radar charts, trend lines) to show topic gaps and learning trajectories.
Immersive Roadmap: Dynamic, database‑driven learning paths that adapt to student progress.
Cross‑Platform UI: Modern, animated Flutter UX with fluid transitions and responsive layouts.
Backend Integrations: Supabase (Postgres) for auth, storage, realtime alerts, plus optional Python microservices for custom inference or heavy logic.
Tech Stack & Architecture:

Frontend: Flutter (Android, iOS, Web) with modern state management and rich animation libraries.
Backend / BaaS: Supabase (PostgreSQL, Auth, Storage, Realtime).
AI Layer: Google Generative AI (Gemini) for responses; a Python microservice handles specialized tasks (ngrok used in dev).
Data & Reports: CSV import/export, PDF report generation, and storage of OCR images & results.
Quick Start (developer):

Install deps: flutter pub get
Run app: flutter run (choose an emulator or device)
Supabase: create a Supabase project, run provided SQL schema scripts, and configure your SUPABASE_URL / SUPABASE_KEY in the app environment.
AI / Microservices: start the Python backend (if used) and expose locally with ngrok during development, then point the app to the service endpoint.
Why this repo matters:

Student‑centered: Focuses on measurable learning improvement, not just content delivery.
Extendable: Modular frontend + backend allows adding subjects, question banks (CSV), and new AI skills.
Production‑ready patterns: Built with deployable Flutter targets and a proven BaaS backend for rapid iteration.
