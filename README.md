# CrewAI Machine Learning Assistant

## Overview

The CrewAI Machine Learning Assistant is a Streamlit application designed to kickstart your machine learning projects. It leverages a team of AI agents to guide you through the initial steps of defining, assessing, and solving machine learning problems.

## Features

- **Problem Definition**: Clarify the machine learning problem you want to solve, identifying the type of problem (e.g., classification, regression) and any specific requirements.

- **Data Assessment**: Evaluate the data provided by the user, assessing its quality, suitability for the problem, and suggesting preprocessing steps if necessary.

- **Model Recommendation**: Suggest the most suitable machine learning models based on the problem definition and data assessment, providing reasons for each recommendation.

- **Starter Code Generation**: Generate starter Python code for the project, including data loading, model definition, and a basic training loop, based on findings from the problem definitions, data assessment, and model recommendation.

## Usage

### Setup

1. **Create a virtual environment (recommended)**
   ```bash
   python -m venv crewai_venv
   ```

2. **Activate the virtual environment**
   
   On Linux/macOS:
   ```bash
   source crewai_venv/bin/activate
   ```
   
   On Windows:
   ```bash
   crewai_venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure your Groq API key**
   
   Create a `.streamlit/secrets.toml` file in the project directory:
   ```bash
   mkdir -p .streamlit
   ```
   
   Add your Groq API key to `.streamlit/secrets.toml`:
   ```toml
   GROQ_API_KEY = "your-groq-api-key-here"
   ```
   
   Get your API key from [https://console.groq.com/keys](https://console.groq.com/keys)

5. **Run the Streamlit app**
   ```bash
   streamlit run app.py
   ```
   
   The app will open in your browser at `http://localhost:8501`

### Using the App

1. Use the sidebar to customize the model selection.

2. Describe your machine learning problem in the provided text input.

3. Optionally, upload a sample .csv of your data.

4. The app will provide a clear problem definition, data assessment, model recommendations, and starter Python code.
