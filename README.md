# Django Sentiment Analysis Application

## Overview

This Django-based web application analyzes the sentiment of user-provided text, determining whether the expressed opinion is positive, negative, or neutral.

## Features

- **Text Sentiment Analysis**: Input text to receive an analysis indicating positive, negative, or neutral sentiment.
- **Visualization**: View text representations of sentiment.

## Requirements

### Software Requirements
- **Python**: 3.8+
- **Django**: 4.0+
- **NLTK**: Natural Language Toolkit for text processing
- **VADER Sentiment Analyzer**: For sentiment analysis
- **Other Dependencies**: Listed in `requirements.txt`

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/AllaUjwalSai/django-sentiment-analysis.git
   cd django-sentiment-analysis
   ```

2. **Set Up a Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply Migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Download NLTK Data**:
   Ensure NLTK data required for sentiment analysis is downloaded:
   ```python
   import nltk
   nltk.download('vader_lexicon')
   ```

6. **Run the Development Server**:
   ```bash
   python manage.py runserver
   ```
   Access the application at `http://127.0.0.1:8000`.

## Usage
1. **Analyze Text**:
   - Navigate to the "Analyze Text" page.
   - Enter the text you wish to analyze.
   - Submit to receive the sentiment analysis results.
   - 
2. **View Analysis History**:
   - Access the "History" page to review your past analyses.

## Project Structure

```
project/
├── sentiment_app/       # Main Django app
├── static/              # Static files (CSS, JS, images)
├── templates/           # HTML templates
├── media/               # Uploaded files
├── requirements.txt     # Dependencies
└── manage.py            # Django management script
```

## Key Components

- **Sentiment Analysis**: Utilizes NLTK's VADER Sentiment Analyzer for evaluating text sentiment.
- **User Interface**: Built with Django templates and styled with Tailwind CSS for a responsive design.
- **Data Visualization**: Incorporates charts to display sentiment distribution.

## Contributing

1. **Fork the Repository**.
2. **Create a Feature Branch**:
   ```bash
   git checkout -b feature-name
   ```
3. **Commit Changes**:
   ```bash
   git commit -m 'Add feature'
   ```
4. **Push to the Branch**:
   ```bash
   git push origin feature-name
   ```
5. **Open a Pull Request**.

## Acknowledgments

- NLTK and the VADER Sentiment Analyzer for providing robust tools for text analysis.
- Django for the web framework.
- Tailwind CSS for styling.

## Contact

For questions or support, contact [AllaUjwalSai] at [ujwalsai16@gmail.com].

