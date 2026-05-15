Starting the app:

1. Environment setup:
```
PORT=2026
```

2. Starting the server:
```
uv run python -m uvicorn main:app --port $PORT --reload
```
- `uv run` – run the following in an environment managed by [uv](https://docs.astral.sh/uv/)
- `python -m uvicorn` – start the [uvicorn](https://uvicorn.dev/) server
- `main:app` – (for uvicorn): import `app` from the `main` module
- `--port $PORT` – listen on defined port
- `--reload` – automatically restart the server when code changes are detected

3. Sending a request:
```
PORT=2026 # Just in case

curl -X POST "http://localhost:$PORT/users" \
  -H "Content-Type: application/json" \
  -d '{
    "username": "magda_gessler",
    "password": "kuchennerewolucje123"
  }'
```
