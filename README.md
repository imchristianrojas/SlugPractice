# SlugPractice

SlugPractice is an innovative tool designed to automatically generate practice problems to aid in academic study. It allows users to create custom flashcards tailored to specific subjects and difficulty levels.

## Features

- Generate practice questions based on user-provided topics and examples
- Adjustable difficulty levels (Easy, Medium, Hard)
- Multiple question formats (Simple Q&A, Multiple Choice, True/False)
- Interactive flashcard interface
- Responsive design for various screen sizes

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/slugpractice.git
   cd slugpractice
   ```

2. Set up a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory and add your OpenAI API key:
   ```
   OPENAI_SLUG_PRACTICE_API_KEY=your_api_key_here
   ```

## Usage

1. Start the Flask server:
   ```
   python app.py
   ```

2. Open a web browser and navigate to `http://127.0.0.1:5000`

3. Enter a subject, an example question, select the difficulty level and question format, then click "Generate" to create flashcards.

4. Use the navigation buttons to move between flashcards and click on a card to reveal the answer.

## Project Structure

- `app.py`: Main Flask application file
- `app/controllers/`: Contains API and user validation controllers
- `app/services/`: Houses the service logic for generating questions
- `static/`: Contains CSS and JavaScript files
- `templates/`: Holds the HTML templates
- `test/`: Includes test files for various components

## Technologies Used

- Backend: Flask (Python)
- Frontend: HTML, CSS, JavaScript (with jQuery)
- API: OpenAI GPT-4 for question generation

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements

- OpenAI for providing the GPT-4 API
- Flask team for the excellent web framework
- All contributors and testers of SlugPractice
