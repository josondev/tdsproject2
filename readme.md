# Tools in Data Science Project

## Overview
This project provides a data science toolset with an interactive GUI for processing various data analysis tasks and queries. The system can handle different types of questions and file uploads for analysis.

## Getting Started

### Prerequisites
- Python 3.7+
- Virtual environment (recommended)

### Installation
Run these commands to set up and start the project:

1. Create a virtual environment:
```
python3 -m venv venv
```

2. Activate the virtual environment:
```
source venv/bin/activate
```

3. Install dependencies:
```
pip install -r requirements.txt
```

4. Update requirements file:
```
pip freeze > requirements.txt
```

5. Start the application:
```
uvicorn main:app --reload
```

Then open your browser and navigate to http://localhost:8000

## Using the Application

### GUI Interface (Recommended)
For the best experience with rich formatted output, use the web interface:

1. Open your browser and navigate to http://localhost:8000
2. Enter your data science question in the text area
3. Upload any relevant files if needed
4. Click "Submit" to process your request
5. View the formatted results in the response section

### API Usage
While the application supports API calls via curl or other HTTP clients, **the GUI provides a superior experience** with:

- Better formatted output
- Easier file uploads
- Visual feedback during processing
- Properly rendered results

Example API call (GUI better):
```
curl -X POST "https://your-app.vercel.app/api/" \
  -H "Content-Type: multipart/form-data" \
  -F "question=Download and unzip file abcd.zip which has a single extract.csv file inside. What is the value in the "answer" column of the CSV file?" \
  -F "file=@abcd.zip"
```

## Features
- Text/Data analysis
- File processing
- Various data science utilities

## Documentation
For more details on specific features and capabilities, refer to the project documentation.