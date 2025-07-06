# GenAI Project Demo

This repository is a play-by-play journal and codebase of a rapid 10-hour hackathon where I led two teammates to build an end-to-end GenAI prototype.

## Project Requirements

### Functional Requirements

1. **Core Chat Flow**: Accept user questions, call the OpenAI GPT-4 API, and display answers.
2. **AI-Driven Health Alert**: Use a few-shot prompt to classify questions as `ALERT` or `SAFE`. On `ALERT`, show a medical warning and skip the chat flow.
3. **Nearby Clinic Finder**: Let users enter a location (address or latitude/longitude). Call Google Places API to find up to 5 open veterinary care clinics and show name, address, and rating.
4. **Example Scenarios**: Provide a dropdown of preset questions (e.g., "midnight vomiting", "teaching cat a scratching post").
5. **Persistence & Sidebar**: Store each Q\&A pair in Supabase. Display the latest 5 entries in the sidebar.
6. **Error Handling & Loading Indicators**: Wrap all external calls in try/catch, show `st.spinner` during requests, and use `st.error` or `st.warning` on exceptions.

### Non-Functional Requirements

1. **Configuration**: Manage API keys and service URLs via environment variables (`OPENAI_API_KEY`, `GOOGLE_PLACES_API_KEY`, `SUPABASE_URL`, `SUPABASE_KEY`).
2. **Project Structure**: Keep code modular with separate files for classification, service integrations, and the main Streamlit app. Store core prompts in `prompts/`.
3. **Documentation**: Provide a clear `README.md` and a replication guide in `REPRODUCE.md`.
4. **Collaboration**: Include a license, issue and pull-request templates, and CI status badges.
5. **Deployment**: Optionally provide Docker or CI/CD scripts for one-command deployment.

## Getting Started

```bash
# Clone the repository
git clone https://github.com/your_username/genai-project-demo.git
cd genai-project-demo

# Install dependencies
pip install -r requirements.txt

# Set environment variables
export OPENAI_API_KEY=YOUR_OPENAI_KEY
export GOOGLE_PLACES_API_KEY=YOUR_GOOGLE_KEY
export SUPABASE_URL=YOUR_SUPABASE_URL
export SUPABASE_KEY=YOUR_SUPABASE_KEY

# Run the app
streamlit run app.py
```

## Project Timeline & Breakdown

For detailed module breakdown and timeboxing, see `docs/THOUGHTS.md`.
