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

The JavaScript code can be written in two equivalent ways. Here's the traditional function notation with detailed comments:
```javascript
function sayHello() {
    fetch('/hello')                          // Makes GET request to /hello endpoint
        .then(function(response) {           // Handles the response
            return response.text();          // Converts response to text
        })
        .then(function(text) {              // Handles the text
            document.getElementById('message').textContent = text;  // Updates page
        });
}
```

And here's the same code using modern arrow function notation, which is more concise:
```javascript
function sayHello() {
    fetch('/hello')                          // Makes GET request to /hello endpoint
        .then(response => response.text())    // Arrow function to handle response
        .then(text => document.getElementById('message').textContent = text);  // Arrow function to update page
}
```

Both versions do exactly the same thing:
1. Makes a GET request to the `/hello` endpoint
2. Converts the response to text
3. Updates the page by setting the text content of the element with id="message"

The arrow function notation (`=>`) is a shorter way to write functions in JavaScript. It's particularly useful for short callback functions like these. The two notations are equivalent, but arrow functions are more commonly used in modern JavaScript.

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