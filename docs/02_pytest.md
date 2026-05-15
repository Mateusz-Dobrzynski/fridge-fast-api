# 2. Ensuring code quality with pytest ✅

## Checking out to a relevant commit
```
git checkout 4c835b7
```

## Directory structure (simplified)
```
.
├── README.md
├── src
│   ├── __init__.py
│   ├── main.py
├── test
│   ├── __init__.py
│   ├── test_misc.py
│   └── test_users.py
├── pyproject.toml
└── uv.lock
```

- `__init__.py` – for proper imports and tests discovery (see [reference](https://www.geeksforgeeks.org/python/what-is-__init__-py-file-in-python/))

## Running pytest with uv

Install pytest:
```
uv add pytest
```

Run tests:
```
uv run pytest
```
