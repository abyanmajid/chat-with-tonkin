# Chat with Tonkin

A simple RAG proof-of-concept for Tonkin built via n8n and vibe-coding.

## Quickstart

### Prerequisites

This quickstart guide assumes you have the following installed on your machine:

- Python >= v3
- Node >= v22
- NPM >= v11

### Local Setup

1. Run n8n locally (this will also install it if you don't yet have it):

```
npx n8n
```

2. Copy the contents of `n8n.json` and import it to a new, empty n8n workflow

3. The n8n workflow is configured to use the following external services: (1) Google Drive, (2) AWS Bedrock, and, and (3) OpenAI. You need to configure your secrets for each and every one of these services to make the workflow run. Please consult the relevant n8n documentation.

4. Clone the repository locally

```
git clone https://github.com/abyanmajid/chat-with-tonkin.git
cd chat-with-tonkin
```

5. Create a Python virtual environment and install UI dependencies

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

6. Serve the UI

```
streamlit run ui.py
```