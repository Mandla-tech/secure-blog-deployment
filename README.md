# secure-blog-deployment
What This Project Demonstrates
This isn't just another "Hello World" deployment. This project showcases real-world DevSecOps challenges and their solutions:

- **Security-First Development:** Automated vulnerability scanning with Snyk
- **Container Security:** Proper Dockerfile configuration for cloud deployment
- **Cloud-Native Deployment:** Google Cloud Run with proper IAM and security controls
- **Real Troubleshooting:** Solving actual deployment issues (port mismatches, permissions) [Blog page](https://iammandla.hashnode.dev/)
- **Complete Pipeline:** From local development to live production environment

# Architecture Overview

graph LR
    A[Local Development] --> B[Docker Container]
    B --> C[Docker Hub Registry]
    C --> D[Google Cloud Run]
    E[GitHub Actions] --> F[Snyk Security Scan]
    F --> B

# 🛠️ Tech Stack

| Component          | Technology        | Purpose                                   |
|:-----------------:|:----------------:|:----------------------------------------:|
| Backend           | Python Flask      | Lightweight web framework                |
| Containerization  | Docker            | Application packaging and isolation      |
| Registry          | Docker Hub        | Container image storage                  |
| Cloud Platform    | Google Cloud Run  | Serverless container deployment          |
| Security Scanning | Snyk              | Vulnerability detection in dependencies |
| CI/CD             | GitHub Actions    | Automated testing and security checks    |
| Monitoring        | Google Cloud Logging | Application and deployment monitoring |

# 📁 Project Structure

secure-blog/
├── app.py                 # Flask application
├── templates/
│   └── home.html         # HTML template with responsive design
├── static/
│   └── css/
│       └── style.css     # Modern CSS styling
├── Dockerfile            # Multi-stage container build
├── requirements.txt      # Python dependencies
├── .github/
│   └── workflows/
│       └── ci.yml       # Security-focused CI pipeline
└── README.md            # This file

# Live Demo
[View Demo Here](https://secure-blog-547606477313.us-central1.run.app/)

# 📝 Blog Series
I've documented this entire journey in a detailed blog series covering:

- DevSecOps principles in action
- Real deployment challenges and solutions
- Security-first development mindset
- Cloud-native best practices

# 🤝 Contributing
While this is primarily a demo/sample project, I welcome:

- Security improvement suggestions
- Code review feedback
- DevSecOps best practice recommendations
 