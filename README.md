# DevOpsCourse

dev ops course repository

## About

A simple Flask web application demonstrating DevOps practices including CI/CD, containerization, and infrastructure as code.

## Features

- Modern UI using Tailwind CSS
- Flask web application
- Docker containerization
- GitHub Actions CI/CD pipeline
- Basic test suite
- Infrastructure as Code (Terraform)

## Prerequisites

- Python 3.9+
- Docker
- GitHub account
- DockerHub account (for container registry)

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/devops-project.git
cd devops-project
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the application:
```bash
python app.py
```

5. Run tests:
```bash
pytest
```

## Docker Deployment

1. Build the Docker image:
```bash
docker build -t devops-project .
```

2. Run the container:
```bash
docker run -p 5000:5000 devops-project
```

## CI/CD Pipeline

The project includes a GitHub Actions workflow that:
1. Runs tests on every push and pull request
2. Builds and pushes Docker image to DockerHub on main branch pushes

To set up the CI/CD pipeline:
1. Fork this repository
2. Add your DockerHub credentials as GitHub Secrets:
   - `DOCKERHUB_USERNAME`
   - `DOCKERHUB_TOKEN`

## Project Structure

```
.
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── Dockerfile         # Container configuration
├── test_app.py        # Test suite
├── templates/         # HTML templates
│   └── index.html
└── .github/
    └── workflows/     # GitHub Actions workflows
        └── ci-cd.yml
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
