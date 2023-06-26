# YouTube Script Generator

Welcome to the repository of YouTube Script Generator. This project utilizes various key components, including Langchain, ChatGPT, Streamlit, and WikipediaAPI.

## Overview

The YouTube Script Generator application demonstrates the powerful capabilities of ChatGPT when combined with Langchain. By leveraging Langchain, the development of language generation models is accelerated, allowing for efficient script generation for YouTube videos.

## Key Components

The following key components are utilized in this project:

- **Langchain**: Langchain is a library that provides utility functions for working with language generation models. It enhances the capabilities of ChatGPT and facilitates prompt-based generation of video titles and scripts.
- **ChatGPT**: ChatGPT is a language model developed by OpenAI. It powers the script generation process and enables natural language conversations.
- **Streamlit**: Streamlit is a framework used for building interactive web applications. It provides the user interface for the YouTube Script Generator, allowing users to input prompts and view the generated titles and scripts.
- **WikipediaAPI**: WikipediaAPI is a wrapper that allows the application to access the Wikipedia API. It enriches the script generation process by incorporating relevant information from Wikipedia.

## Usage

To use the YouTube Script Generator application, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/saadashraf1/youtube-script-generator.git
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the environment variables:
   - Obtain an API key from OpenAI and set it as `OPENAI_API_KEY` in the environment.
   - Make sure to replace `apikey` in the `apikey.py` file with your actual API key.

4. Run the application:
   ```bash
   streamlit run app.py
   ```

5. Access the application in your web browser at `http://localhost:8501`.

6. Enter your desired prompt in the provided text input field. The application will generate a YouTube video title and script based on the input.

7. The generated title, script, and Wikipedia research (if applicable) will be displayed on the screen. You can also view the history of generated titles and scripts.

## Customization

The YouTube Script Generator application can be customized according to your needs:

- Modify the prompt templates in the code (`title_template` and `script_template`) to adjust the generation behavior.
- Adjust the temperature of the ChatGPT model to control the creativity of the generated content.
- Customize the Streamlit user interface to enhance the user experience.

Feel free to explore the code and make any necessary modifications to suit your requirements.


## License

This project is licensed under the [MIT License](LICENSE).


## Running the Application

Once the application is running, a web interface will be displayed with a text input field labeled "Plug in your prompt here". Enter your desired prompt in this field.

The application uses prompt templates to generate video titles and scripts. The following templates are defined:
- `title_template`: Generates a YouTube video title based on the provided topic.
- `script_template`: Generates a YouTube video script based on the provided title and Wikipedia research.

The application also utilizes conversation buffers to remember previous inputs. Two buffers are defined:
- `title_memory`: Stores previous topics for generating titles.
- `script_memory`: Stores previous titles for generating scripts.

If a prompt is provided, the application will generate a title and script based on the input. The generated title, script, and Wikipedia research will be displayed on the screen.

The application also provides expandable sections to view the history of generated titles, scripts, and Wikipedia research.

