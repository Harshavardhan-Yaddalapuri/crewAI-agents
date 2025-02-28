# Blog Post Content Creation Crew

This project uses the `crewai` library to automate the process of creating a blog post. The script defines agents for planning, writing, and editing a blog post, and then executes these tasks in sequence.

## Prerequisites

Before you can run the script, you need to have the following installed:

- Python 3.7 or higher
- `crewai` library
- An API key for OpenAI

## Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/content-writing-crew.git
    cd content-writing-crew
    ```

2. **Create a virtual environment:**

    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install the required packages:**

    ```sh
    pip install crewai crewai_tools
    ```
 

4. **Set up your OpenAI API key:**

    You need to set the `OPENAI_API_KEY` environment variable with your OpenAI API key. If you are using a `.env` file, you can add the following line to it:

    ```sh
    OPENAI_API_KEY='your_openai_api_key'
    ```

    Make sure to load the environment variables from the `.env` file in your script. You can use the `python-dotenv` package to do this. First, install the package:

    ```sh
    pip install python-dotenv
    ```

    Then, add the following lines to your script to load the environment variables:

    ```python
    from dotenv import load_dotenv
    import os

    load_dotenv()
    api_key = os.getenv('OPENAI_API_KEY')
    ```


## Running the Script

To run the script, use the following command:

```sh
python BlogPostContentCreationCrew.py