# Math Hand Gesture Recognition

This project combines computer vision and AI to create a virtual calculator that recognizes hand gestures to solve mathematical problems drawn in the air.

## Features

- Draw mathematical equations with your index finger
- Clear the canvas with a simple thumb gesture
- Get instant solutions by triggering the AI with a four-finger gesture
- Real-time hand tracking using MediaPipe
- AI-powered math problem solving with Google's Gemini

## Prerequisites

- Python 3.11
- A webcam
- Google Generative AI API key ([Get it here](https://ai.google.dev/))

## Setup Instructions

### 1. Create and activate a virtual environment

```bash
uv venv --python 3.11
.venv\Scripts\activate
```

### 2. Install requirements

```bash
uv pip install -r requirements.txt
```

### 3. Configure your API key

Open `math_gestures.py` and replace `"Your API Key"` with your actual Google Generative AI API key on line 49:

```python
genai.configure(api_key="Your API Key")
```

### 4. Run the application

```bash
streamlit run math_gestures.py
```

## How to Use

- **Draw**: Extend only your index finger to draw on the canvas
- **Clear**: Extend only your thumb to clear the canvas
- **Solve**: Extend all fingers except thumb to send the drawing to the AI for solving

## Technologies Used

- OpenCV: Computer vision and image processing
- MediaPipe: Hand tracking and gesture recognition
- Streamlit: Interactive web interface
- Google Generative AI (Gemini): AI-powered math problem solving
