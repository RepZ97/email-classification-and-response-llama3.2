# Email Classification and Response Automation

This project aims to classify and respond to emails using AI agents. The project utilizes `llama 3.2` model and `crewai` to create agents for classifying emails based on their importance and responding accordingly.

## Project Overview

The project consists of two main agents:
1. **Email Classifier**: Classifies emails into three categories: important, casual, or spam.
2. **Email Responder**: Responds to emails based on their classification.

### Agents

- **Classifier Agent**:
  - **Role**: Email classifier
  - **Goal**: Accurately classify emails based on their importance.
  - **Backstory**: An AI assistant focused on classifying emails accurately and honestly.

- **Responder Agent**:
  - **Role**: Email responder
  - **Goal**: Write concise responses to emails based on their importance.
  - **Backstory**: An AI assistant tasked with writing short responses based on email importance provided by the classifier agent.

### Tasks

- **Classify Email**:
  - **Description**: Classify the provided email.
  - **Expected Output**: One of these three options: `important`, `casual`, or `spam`.

- **Respond to Email**:
  - **Description**: Respond to the email based on its importance.
  - **Expected Output**: A concise response based on the email's classification.

## Installation

1. Download and install Ollama
  ```
  https://ollama.com/download/OllamaSetup.exe
  ```

2. Pull llama 3.2 model
  ```sh
  ollama run llama3.2
  ```

3. Run the model as a server in localhost
  ```sh
  ollama serve
  ```

4. Clone the repository:
    ```sh
    git clone https://github.com/RepZ97/email-classification-and-response-llama3.2.git
    cd email-classification-and-response-llama3.2
    ```

5. Create a virtual environment and activate it:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

6. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

7. Install `crewai` if not already installed:
    ```sh
    pip install crewai
    ```

## Usage

To run the email classification and response workflow:

1. Ensure you have `ollama/llama3.2` model installed.
2. Execute the `main.py` script:
    ```sh
    python main.py
    ```
