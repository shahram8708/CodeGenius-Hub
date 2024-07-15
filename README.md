# CodeGenius Hub

CodeGenius Hub is a web application designed to help users input code, receive immediate feedback on its output and correctness, and identify any errors. The platform streamlines the debugging and learning process by providing corrected versions of code that are accurate and complete.

## Features

- **Code Input:** Users can input code into a text area.
- **Code Analysis:** The application analyzes the code, identifies errors, and explains them.
- **Code Correction:** Provides a corrected version of the code.
- **Code Output:** Displays the output of the code.
- **Copy to Clipboard:** Users can copy the code suggestions to the clipboard.
- **Device Check:** Alerts users if they are not using a desktop, laptop, or MacBook.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (jQuery)
- **Backend:** Flask, Python
- **API:** Google Gemini API

## Installation

1. **Clone the repository:**

   ```sh
   git clone https://github.com/shahram8708/codegenius-hub.git
   cd codegenius-hub
   ```

2. **Create a virtual environment:**

   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the dependencies:**

   ```sh
   pip install -r requirements.txt
   ```

## Configuration

1. **Set up the API Key:**

   Replace the `API_ENDPOINT` in `app.py` with your Google Gemini API key.

   ```python
   API_ENDPOINT = "https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=YOUR_API_KEY"
   ```

## Usage

1. **Run the application:**

   ```sh
   python app.py
   ```

2. **Open your web browser:**

   Navigate to `http://127.0.0.1:5000` to access the CodeGenius Hub.

## File Structure

```
codegenius-hub/
├── static/
│   └── css/
│       └── style.css
├── templates/
│   ├── index.html
│   └── unsupported.html
├── app.py
├── requirements.txt
└── README.md
```

## API Reference

- **Endpoint:** `/search`
  - **Method:** POST
  - **Parameters:**
    - `search_query` (string): The code prompt input by the user.
  - **Response:**
    - `success` (boolean): Indicates if the request was successful.
    - `code_suggestion` (string): The generated code suggestion.
    - `error` (string): Error message if the request was not successful.

## Contributing

1. **Fork the repository.**
2. **Create a new branch:**

   ```sh
   git checkout -b feature
   ```

3. **Make your changes and commit them:**

   ```sh
   git commit -m
   ```

4. **Push to the branch:**

   ```sh
   git push origin feature
   ```

5. **Create a pull request.**

## License

This project is licensed under the MIT License.

## Contact

- **Author:** Shah Ram
- **Email:** shahram8708@gmail.com
- **GitHub:** [Shah Ram](https://github.com/shahram8708)
