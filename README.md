[![Python application test with Github Actions](https://github.com/python-dev-og/CICD-API-microservices/actions/workflows/devops.yml/badge.svg)](https://github.com/python-dev-og/CICD-API-microservices/actions/workflows/devops.yml)
![GitHub last commit](https://img.shields.io/github/last-commit/python-dev-og/CICD-API-microservices)
![GitHub issues](https://img.shields.io/github/issues/python-dev-og/CICD-API-microservices)
![GitHub stars](https://img.shields.io/github/stars/python-dev-og/CICD-API-microservices)
![GitHub forks](https://img.shields.io/github/forks/python-dev-og/CICD-API-microservices)
![Python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)


# Wikipedia API Microservice

## Introduction
This Python microservice, built using FastAPI, serves as a lightweight interface to interact with Wikipedia. It enables users to search for terms, retrieve specific Wikipedia pages, and extract important phrases from these pages.

## Getting Started

### Prerequisites
Before you begin, ensure you have the following installed:
- Python 3.x
- pip (Python package installer)

### Installation
To install and run this microservice on your local machine, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/python-dev-og/CICD-API-microservices.git
   ```

2. **Navigate to the Project Directory:**
   ```bash
   cd [Your Project Directory]
   ```

3. **Install Dependencies:**
   - FastAPI: A modern, fast web framework for building APIs with Python.
   - Uvicorn: An ASGI server for running FastAPI applications.
   - Wikipedia-API: A Python wrapper for Wikipedia's search and content APIs.
   - TextBlob: A library for processing textual data.
   
   Run the following command to install these packages:
   ```bash
   pip install fastapi uvicorn wikipedia-api textblob
   ```

### Running the Application
After installing the dependencies, you can start the server with this command:
```bash
uvicorn main:app --reload
```
The `--reload` flag enables auto-reloading of the server on code changes.

## Usage

### API Endpoints
Access the following endpoints through your browser or an API testing tool like Postman:

- **Root Endpoint (`GET /`):**
  Returns a welcome message and API usage instructions.

- **Search Wikipedia (`GET /search/{value}`):**
  Search for a term in Wikipedia. Replace `{value}` with your search term.

- **Retrieve Wikipedia Page (`GET /wiki/{name}`):**
  Fetch a specific Wikipedia page. Replace `{name}` with the name of the page.

- **Retrieve Phrases (`GET /phrase/{name}`):**
  Extract key phrases from a Wikipedia page. Replace `{name}` with the name of the page.

### Examples
- To search Wikipedia for "Python":
  ```
  http://localhost:8080/search/Python
  ```

- To retrieve the Wikipedia page for "Python":
  ```
  http://localhost:8080/wiki/Python
  ```

- To extract phrases from the Wikipedia page "Python":
  ```
  http://localhost:8080/phrase/Python
  ```

## Dependencies
List of Python packages required:
- FastAPI
- Uvicorn
- Wikipedia-API
- TextBlob

## Contributing
Contributions to improve the application are welcome. Please follow these steps to contribute:
1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License
MIT License

---

Happy Coding!
```
