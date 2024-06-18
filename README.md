# AI-Driven Insurance Information Retrieval and Summarization System

Welcome to the AI-Driven Insurance Information Retrieval and Summarization System! This project utilizes the LangChain framework and Retrieval-Augmented Generation (RAG) to efficiently retrieve and summarize insurance-related information from various sources, including web sources, research papers, and user-provided documents.

## Features

- **Integration with Wikipedia and Arxiv APIs**: Fetches relevant information efficiently.
- **FAISS for Vector Storage**: Utilizes FAISS for storing vectors and quick information retrieval.
- **LangChain Framework**: Enhances the system's ability to link together multiple language models and retrieval mechanisms.
- **Insurance Website Database**: Option to add links to insurance website databases for more comprehensive data retrieval.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Adding Insurance Website Database](#adding-insurance-website-database)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Steps

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/insurance-info-retrieval.git
    cd insurance-info-retrieval
    ```

2. **Create and Activate Virtual Environment**

    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**

    ```sh
    pip install -r requirements.txt
    ```

4. **Set Up API Keys**

    Create a `.env` file in the root directory and add your API keys for Wikipedia and Arxiv:

    ```plaintext
    WIKIPEDIA_API_KEY=your_wikipedia_api_key
    ARXIV_API_KEY=your_arxiv_api_key
    ```

## Usage

1. **Run the Application**

    ```sh
    python app.py
    ```

2. **Interacting with the System**

    - Input your query related to insurance.
    - The system will retrieve and summarize information from Wikipedia, Arxiv, and your own documents.

## Adding Insurance Website Database

To enhance the system's capabilities, you can add links to insurance website databases. Follow these steps:

1. **Create a File**

    Create a file named `insurance_websites.txt` in the `data/` directory.

2. **Add Links**

    Add your insurance website database links in the `insurance_websites.txt` file, each link on a new line.

    ```plaintext
    https://www.exampleinsurance1.com
    https://www.exampleinsurance2.com
    ```

3. **Update Configuration**

    Ensure the system reads from this file to include these websites in the information retrieval process.

## Project Structure

- `app.py`: Main application file to run the system.
- `config.py`: Configuration settings for API keys and other parameters.
- `data/`: Directory to store user documents and other data.
- `models/`: Directory containing model-related code and configurations.
- `requirements.txt`: List of required Python packages.
- `insurance_websites.txt`: File containing insurance website database links.
- `README.md`: This file.

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License

This project is licensed under the MIT License.
