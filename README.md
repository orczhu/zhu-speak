# How to run

Requires Python 3.8+.

1. Install dependencies:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

2. Create a `.env` file in the repo root:

   ```
   OPENAI_API_KEY=your-openai-api-key
   # Optional, only needed for the "x.ai Grok" model option
   XAI_API_KEY=your-xai-api-key
   ```

3. Start the server:

   ```bash
   uvicorn realtime_server:app --host 127.0.0.1 --port 3005
   ```

4. Open http://localhost:3005, allow microphone access, and click **Start**.

## Tests

```bash
pytest tests/
```
