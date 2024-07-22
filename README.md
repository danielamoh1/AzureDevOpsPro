# AzureDevOpsPro

# AzureDevOpsPro

Welcome to the AzureDevOpsPro repository. This project demonstrates a highly complex CI/CD pipeline setup using Azure DevOps and GitHub.

![azure-devops-ci-cd-architecture](https://github.com/user-attachments/assets/2f672f3c-c696-4041-a9b5-187e3a3e7ae4)

## Project Structure

- `src/`: Contains the main application code and utility libraries.
- `tests/`: Contains unit and integration tests.
- `.azure-pipelines/`: Contains Azure DevOps pipeline configurations for CI, PR, and CD.
- `docs/`: Documentation including architecture diagrams and requirements.
- `scripts/`: Deployment scripts.
- `requirements.txt`: Lists Python package dependencies.
- `README.md`: This file.

## Getting Started

### Prerequisites

- Python 3.6 or later
- Azure DevOps Account
- GitHub Account

### Setup

1. **Clone the repository:**

    ```
    git clone https://github.com/yourusername/AzureDevOpsPro.git
    cd AzureDevOpsPro
    ```

2. **Create a virtual environment:**

    ```
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies:**

    ```
    pip install -r requirements.txt
    ```

4. **Run the application:**

    ```
    python src/app/main.py
    ```

5. **Run tests:**

    ```
    pytest tests/unit
    pytest tests/integration
    ```

## Azure DevOps Pipelines

### CI Pipeline (`azure-pipelines-ci.yml`)

This pipeline runs on every commit to the `main` branch and includes linting, unit tests, and integration tests.

### PR Pipeline (`azure-pipelines-pr.yml`)

This pipeline runs on pull requests and includes linting and unit tests.

### CD Pipeline (`azure-pipelines-cd.yml`)

This pipeline runs on successful builds and deploys the application using a deployment script.

To set up the pipelines:

1. Go to [Azure DevOps](https://dev.azure.com/) and sign in with your account.
2. Create a new project or navigate to your existing project.
3. Go to Pipelines and create new pipelines for CI, PR, and CD using the corresponding YAML files.
