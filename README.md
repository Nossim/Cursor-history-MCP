# Cursor History MCP 📜

![Cursor History MCP](https://img.shields.io/badge/Cursor%20History%20MCP-v1.0.0-blue.svg)
![API](https://img.shields.io/badge/API-FastAPI-orange.svg)
![Docker](https://img.shields.io/badge/Docker-Container-blue.svg)
![LanceDB](https://img.shields.io/badge/LanceDB-Vector%20Database-green.svg)

## Overview

Welcome to the **Cursor History MCP** repository! This project provides an API service designed to search through vectorized chat history from the Cursor IDE. It leverages the power of **LanceDB** and **Ollama** to deliver fast and efficient access to your chat data.

### Features

- **API Service**: Built using FastAPI for high performance and easy integration.
- **Vectorized Search**: Utilizes embeddings to enhance search capabilities.
- **Self-Hosted**: You can run this service locally or on your own server.
- **Docker Support**: Easy to deploy with Docker.
- **Integration with Ollama**: Access local LLM models for advanced processing.

## Getting Started

To get started with **Cursor History MCP**, follow these steps:

### Prerequisites

Make sure you have the following installed:

- Docker
- Python 3.8 or higher
- FastAPI
- LanceDB
- Ollama

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Nossim/Cursor-history-MCP.git
   cd Cursor-history-MCP
   ```

2. Build the Docker image:

   ```bash
   docker build -t cursor-history-mcp .
   ```

3. Run the Docker container:

   ```bash
   docker run -p 8000:8000 cursor-history-mcp
   ```

4. Access the API at `http://localhost:8000/docs` to explore the endpoints.

### Downloading Releases

To get the latest version, visit the [Releases](https://github.com/Nossim/Cursor-history-MCP/releases) section. Download the required file and execute it to set up your environment.

## Usage

Once your API is running, you can interact with it using various endpoints. Here are some key endpoints:

### Search Chat History

- **Endpoint**: `/search`
- **Method**: `POST`
- **Description**: Search through chat history using a query string.

#### Request Body

```json
{
  "query": "Your search query here"
}
```

#### Response

```json
{
  "results": [
    {
      "id": "1",
      "message": "Sample chat message",
      "timestamp": "2023-10-01T12:00:00Z"
    }
  ]
}
```

### Get Chat History

- **Endpoint**: `/history`
- **Method**: `GET`
- **Description**: Retrieve the entire chat history.

#### Response

```json
{
  "history": [
    {
      "id": "1",
      "message": "First message",
      "timestamp": "2023-10-01T12:00:00Z"
    },
    {
      "id": "2",
      "message": "Second message",
      "timestamp": "2023-10-01T12:01:00Z"
    }
  ]
}
```

## Topics

This repository covers several important topics:

- **API**: The core of our service, built on FastAPI.
- **Chat History**: Efficient storage and retrieval of chat data.
- **Docker**: Containerization for easy deployment.
- **Embeddings**: Vectorization of text for enhanced search.
- **FastAPI**: A modern web framework for building APIs.
- **LanceDB**: A vector database optimized for search.
- **Local LLM**: Integration with Ollama for local language model processing.
- **MCP Server**: The main server component of this project.
- **Ollama**: A tool for running local language models.
- **RAG**: Retrieval-Augmented Generation for improved results.
- **Self-Hosted**: Full control over your data and service.
- **Vector Database**: Efficient storage and querying of vectorized data.

## Contributing

We welcome contributions to **Cursor History MCP**! If you want to help improve the project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your fork.
5. Create a pull request.

Please ensure your code adheres to the project's coding standards and includes tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

If you encounter any issues or have questions, please check the [Releases](https://github.com/Nossim/Cursor-history-MCP/releases) section for updates. You can also open an issue in the repository for further assistance.

## Acknowledgments

- Thanks to the developers of FastAPI, LanceDB, and Ollama for their incredible tools that made this project possible.
- Special thanks to the community for their support and feedback.

---

Feel free to explore the repository and make use of the API service. Your feedback is always welcome!