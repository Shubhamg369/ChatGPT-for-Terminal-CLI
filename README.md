# ChatGPT Clone For Terminal/CLI

This is a ChatGPT API integration straight to the terminal/CLI. Here, we're building an interactive chatbot using OpenAI, implemented in Python, and supported by various packages such as Typer for command line interface creation. Follow along to set up and get this project up and running on your machine :)

![Login](https://github.com/Shubhamg369/Private/blob/main/DALL·E%202023-10-22%2012.18.35%20-%20Illustration%20of%20a%20terminal%20floating%20in%20a%20dreamy%2C%20abstract%20space%20filled%20with%20soft%20pastel%20colors.%20The%20terminal's%20screen%20displays%20'ChatGPT_%20Speak%20your%20mi.png)


## Prerequisites

- Python 3.11 (recommended to use `pyenv` for managing Python versions)
- OpenAI API key
- Python packages: `typer`, `python-dotenv`, and others specified in the project

## Setup

### 1. Python Environment Setup

We are using `pyenv` to manage our Python installations and `pyenv-virtualenv` for creating virtual environments. Instructions are provided for macOS. Refer to the official documentation for Windows or Linux installations.

#### Install pyenv:

```bash
brew install pyenv
```

#### Install pyenv-virtualenv:

```bash
brew install pyenv-virtualenv
```

### 2. Project Dependencies

Once you have the appropriate Python version installed and a virtual environment set up, install the project dependencies:

```bash
pip install -r requirements.txt
```

### 3. OpenAI API Key Configuration

You will need an OpenAI API key for this project. Store it securely using environment variables.

```bash
touch .env
echo "OPENAI_API_KEY=your-api-key" >> .env
```

Replace `"your-api-key"` with your actual OpenAI API key.

**Note:** Ensure you have sufficient OpenAI API credits, as each request to the API may incur a cost.

## Project Initialization

Create a directory for the project, set up your virtual environment, and activate it:

```bash
mkdir chatgpt-clone
cd chatgpt-clone
pyenv virtualenv 3.11.0 chatgpt-clone-env
pyenv activate chatgpt-clone-env
```
![Login](https://github.com/Shubhamg369/Private/blob/main/DALL·E%202023-10-22%2012.19.15%20-%20Illustration%20of%20a%20vintage%20terminal%2C%20where%20the%20glow%20from%20the%20green%20text%20illuminates%20the%20surroundings.%20The%20text%20reads%20'ChatGPT_%20Ready%20for%20input'.%20Abstra.png)
## Coding and Running the Chatbot

Now, dive into the code. Start by creating a `main.py` file in your project directory, and import all necessary dependencies. This project uses `typer` for CLI interactions, `python-dotenv` for secure API key storage, and the `openai` package for core functionality.

1. **Setting up the application command**:
   - Use Typer decorators to create interactive command-line applications.

2. **Handling user interactions**:
   - Implement functions to handle user inputs and communicate with the OpenAI API.

3. **Processing API responses**:
   - Parse the JSON responses from the OpenAI API to extract relevant information.

4. **Enhancing chatbot memory**:
   - Implement context handling for more coherent conversation with the chatbot.

5. **Customizing chatbot parameters**:
   - Allow customization of various parameters (e.g., `max_tokens`, `temperature`) directly from the command line.

6. **Optimizing user experience**:
   - Enhance the initialization process to start a conversation immediately upon launching the program.

Run your chatbot:

```bash
python main.py --help  # To display help information and available commands
python main.py --max-tokens 150  # Example command to customize token limit
```

## Licensing

The code in this project is licensed under MIT license.

