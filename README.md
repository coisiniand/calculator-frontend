# Calculator Frontend

This front-end client is designed to work with the Python backend service.

## Features

- Calculator keypad with basic arithmetic operations
- Decimal input and expression editing
- API-based calculation request to the backend
- History display from the backend database
- Delete single record and clear-all history functions

## Requirements

- A modern browser
- The backend running on `http://localhost:8000`

## Start locally

```bash
python -m http.server 8080
```

Then open the page in a browser:

```text
http://localhost:8080
```

The page will call the backend at `http://localhost:8000`.
