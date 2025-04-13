# DevOpsCourse

dev ops course repository

## About

A simple Flask web application demonstrating DevOps practices including CI/CD and testing.

## Features

- Modern UI using Tailwind CSS
- Flask web application
- GitHub Actions CI/CD pipeline
- Basic test suite

## Prerequisites

- Python 3.9+
- GitHub account

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

## CI/CD Pipeline

The project includes a GitHub Actions workflow that:
1. Runs tests on every push and pull request

## Project Structure

```
.
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── test_app.py        # Test suite
└── templates/         # HTML templates
    └── index.html
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
