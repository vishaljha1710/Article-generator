# Article Generator using LangChain API and Python Flask

## Overview

This repository contains a Python Flask application that leverages the LangChain API to generate high-quality articles automatically. With the power of LangChain's natural language processing capabilities, you can create informative and engaging articles on various topics effortlessly.

## Features

- Seamless integration with LangChain API for generating content.
- User-friendly web interface for generating articles.
- Customizable article length and topic selection.
- Real-time preview of generated articles.
- Easy deployment with Docker.

## Prerequisites

Before you get started, ensure you have the following prerequisites:

- Python 3.x installed on your system.
- Docker installed (optional, for deployment).
- LangChain API access credentials (API key).

## Getting Started

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/article-generator.git
   ```

2. Navigate to the project directory:

   ```bash
   cd article-generator
   ```

3. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `config.py` file in the project directory and add your LangChain API key:

   ```python
   # config.py
   LANGCHAIN_API_KEY = "your-api-key-here"
   ```

5. Start the Flask application:

   ```bash
   python app.py
   ```

6. Access the web interface by opening a browser and navigating to `http://localhost:5000`.

## Usage

1. Select a topic for your article.
2. Set the desired article length.
3. Click the "Generate Article" button.
4. The generated article will appear in the preview panel.

## Deployment with Docker

To deploy the application using Docker, follow these steps:

1. Build the Docker image:

   ```bash
   docker build -t article-generator .
   ```

2. Run the Docker container:

   ```bash
   docker run -p 8080:5000 -e LANGCHAIN_API_KEY="your-api-key-here" article-generator
   ```

3. Access the application at `http://localhost:8080` in your web browser.

## Customize

You can customize the application by modifying the Flask templates and stylesheets in the `templates` and `static` directories, respectively.

## Contributing

Contributions to this project are welcome. Please follow the standard GitHub fork and pull request workflow.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Special thanks to LangChain for providing the powerful API for content generation.
- Thanks to the Python Flask community for creating a user-friendly web framework.

Happy article generation!
