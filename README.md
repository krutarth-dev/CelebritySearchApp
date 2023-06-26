# Celebrity Search App

The Celebrity Search App is a web application that allows users to search for information about celebrities. It utilizes the OpenAI API and the Langchain library to generate natural language responses based on user inputs.

## Getting Started

To get started with the Celebrity Search App, follow the instructions below.

### Prerequisites

Make sure you have the following prerequisites installed:

- Python 3.6 or higher
- Streamlit
- OpenAI Python library (installed via pip)

### Installation

1. Clone the repository:

```
git clone <repository_url>
```

2. Install the required dependencies:

```
pip install -r requirements.txt
```

### API Key Setup

Before running the application, you need to set up your OpenAI API key. Follow these steps:

1. Sign up for an OpenAI account and obtain an API key.

2. Open the `app.py` file in a text editor.

3. Set your OpenAI API key as an environment variable:

```python
os.environ["OPENAI_API_KEY"] = "<your_api_key>"
```

Replace `<your_api_key>` with your actual API key.

## Usage

To run the Celebrity Search App, use the following command:

```
streamlit run app.py
```

This will start the application and display a web interface.

1. Enter the name of a celebrity in the text input field.

2. Click the "Search" button to initiate the search.

3. The application will generate information about the celebrity, including their name, date of birth, and major events that happened around their birth date.

4. The results will be displayed on the web interface.

## Customization

You can customize the behavior of the app by modifying the code in the `app.py` file.

- To change the OpenAI temperature value for generating responses, modify the `temperature` parameter when initializing the `OpenAI` object.

- To modify the prompts and templates for generating queries to OpenAI, update the `PromptTemplate` objects and their corresponding chains in the code.

- To change the variables used in the prompts, such as `name`, `person`, or `dob`, modify the `input_variables` and `template` parameters in the `PromptTemplate` objects.

