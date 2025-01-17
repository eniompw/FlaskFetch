# Simple Flask Fetch Demo

A minimal example showing how to use the Fetch API with Flask. This demo shows how to make a simple request from a webpage to a Flask backend.

## What it Does

- Displays a webpage with a button
- When clicked, fetches a message from the Flask server
- Displays the response on the page

## Project Structure 

```
.
├── README.md
├── app.py
├── requirements.txt
└── templates/
    └── index.html
```

## Setup

1. Install Python requirements: 
   ```bash
   pip install -r requirements.txt
   ```

2. Run the Flask app:
   ```bash
   python app.py
   ```

3. Open your browser to `http://127.0.0.1:5000`

## Code Explanation

### Backend (app.py)
- Creates a Flask server with two routes:
  - `/` serves the main webpage
  - `/hello` returns a simple greeting

### Frontend (index.html)
- Shows a button that triggers a fetch request
- Uses the Fetch API to make a request to `/hello`
- Displays the server's response in a paragraph element

## Learning Points

- Basic Flask route setup
- Simple HTML structure
- How to use the Fetch API
- Handling responses from a server
- Updating webpage content with JavaScript

## Next Steps

Try modifying the code to:
- Return different types of messages
- Add more buttons with different actions
- Style the page with CSS
- Add error handling
- Return JSON data instead of plain text 

## References

For more information about the Fetch API:
- [W3Schools - JavaScript Fetch API](https://www.w3schools.com/js/js_api_fetch.asp)
- [MDN Web Docs - Using the Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) 