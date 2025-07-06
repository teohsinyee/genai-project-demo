# Thoughts Journal

This document is a **living journal** capturing my real-time thought process while building an end-to-end GenAI demo. It is updated **after each development slice**. Anyone reading it can:

* See **date-stamped entries** of “what, why, and how” of each decision
* Follow **code references** to commits or files
* Review **challenges, decisions, and next steps** for every slice

Below is the **full project plan** and timeboxed modules, followed by our first sprint entry.

---

## Full 10‑Hour Plan & Module Breakdown

| Module                                 | Time  | Who        | Priority |
| -------------------------------------- | ----- | ---------- | -------- |
| 1. System Prompt & GPT Chat Loop       | 1.0 h | Lead       | Must-Do  |
| 2. AI-Driven Health Alert              | 1.0 h | Lead       | Must-Do  |
| 3. Google Places Clinic Finder         | 1.0 h | Teammate A | Must-Do  |
| 4. Supabase Q\&A Persistence & Sidebar | 1.0 h | Teammate B | Must-Do  |
| 5. Streamlit Frontend & Interaction    | 2.0 h | Teammate C | Must-Do  |
| 6. Error Handling & Loading Spinners   | 0.5 h | All        | Must-Do  |
| 7. Example Question Presets            | 0.5 h | Teammate C | Optional |
| 8. Address Geocoding (Optional)        | 0.5 h | Teammate A | Optional |
| 9. Documentation (README & Reproduce)  | 1.5 h | Lead       | Must-Do  |
| 10. Deployment Scripts (Docker/CI)     | 1.0 h | Lead       | Optional |
| 11. Testing & Bug Fixes                | 1.0 h | All        | Must-Do  |

---
## 2025-07-07 10:00 PM — 1-Hour MVP Slice Kickoff  
- Decided to build only “input → GPT call → render” in 1h  
- Set up Streamlit & OpenAI env, wrote minimal `app.py`  

