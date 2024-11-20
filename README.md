# Basic CREWAI Application

This repository contains a basic Python application to work with the `CREWAI` library. It is structured using Poetry for dependency management and incorporates several powerful tools for web scraping, AI, and Python development.

---

## Prerequisites

1. **Python**: Ensure you have Python 3.12 or later installed.
2. **Poetry**: Poetry is required for managing dependencies and packaging.
3. **Git**: To clone the repository.

---

## Setup Instructions

Follow these steps to set up the application:

### 1. Clone the Repository

```bash
git clone <repository-url>
```
---

## 2. Set Up the Virtual Environment
```bash
python -m venv venv
```
.\venv\Scripts\activate  # Windows

---

## 3. Install Poetry
```bash
pip install poetry
```
---

## 4. Create and Initialize the Project
```bash
poetry new basiccrewai --name app

cd basiccrewai
```
---

##5. Add Dependencies
Install the required dependencies:
```bash
poetry add crewai beautifulsoup4
```
Update the Python version constraint in pyproject.toml:
python = ">=3.12,<=3.13"
Add additional dependencies:
```bash
pip install -U langchain langchain-openai
pip install python-dotenv typing
python.exe -m pip install --upgrade pip
poetry update
poetry add setuptools
```
pyproject.toml Configuration
Below is the updated configuration in pyproject.toml:
```bash
[tool.poetry]
name = "app"
version = "0.1.0"
description = ""
authors = ["felucchesi85 <fernando.lucchesi.gabriel@gmail.com>"]
readme = "README.md"

[tool.poetry.dependencies]
python = ">=3.12,<=3.13"
crewai = "^0.28.8"
beautifulsoup4 = "^4.12.3"
langchain-groq = "^0.1.3"
setuptools = "^75.5.0"

[build-system]
requires = ["poetry-core"]
build-backend = "poetry.core.masonry.api"
```
```bash
pip install python-dotenv typing
```
We can now run the app from terminal
```bash
cd app
poetry run python3 multiagent.py
```

##Usage
Activate the virtual environment:
.\venv\Scripts\activate  # Windows

Run your Python scripts or build the application as needed.

##Troubleshooting
Ensure the correct Python version (>=3.12,<=3.13) is installed.
If dependencies fail to install, try running poetry lock followed by poetry install.
