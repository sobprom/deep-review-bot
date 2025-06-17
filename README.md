# 🤖 Deep Review Bot

**AI-powered code review assistant** with GitLab integration | Powered by DeepSeek Chat

[![GitLab CI](https://img.shields.io/gitlab/pipeline-status/your-username/deep-review-bot)](https://gitlab.com/your-username/deep-review-bot/-/pipelines)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![Java](https://img.shields.io/badge/Java-17+-orange)](https://openjdk.org)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.1-brightgreen)](https://spring.io/projects/spring-boot)

## 🚀 Features

- **Automated Code Reviews** - AI analysis of merge requests
- **Smart Commenting** - Context-aware suggestions
- **Multi-Language Support** - Java, Python, JavaScript and more
- **Security Scanning** - OWASP Top 10 vulnerability detection
- **GitLab Integration** - Seamless workflow with webhooks

## 📦 Installation

### Prerequisites
- Java 17+
- GitLab account
- DeepSeek API key

### Docker Setup
```bash
docker run -d \
  -e DEEPSEEK_API_KEY=your_api_key \
  -e GITLAB_TOKEN=your_gitlab_token \
  -p 8080:8080 \
  ghcr.io/your-username/deep-review-bot:latest
```

## 🔧 Configuration
Add to your `.gitlab-ci.yml`:
```yaml
review:
  stage: test
  script:
    - curl -X POST "${DEEP_REVIEW_URL}/api/review?project_id=${CI_PROJECT_ID}&mr_id=${CI_MERGE_REQUEST_IID}"
  rules:
    - if: $CI_MERGE_REQUEST_ID
```

Set environment variables:
- `DEEPSEEK_API_KEY`: Your DeepSeek Chat API key
- `GITLAB_TOKEN`: GitLab access token with `api` scope

## 🛠 Tech Stack

- **Backend**: Spring Boot 3.1
- **AI Engine**: DeepSeek Chat API
- **Database**: PostgreSQL (for review history)
- **Caching**: Redis
- **CI/CD**: GitLab Pipelines

## 🤝 Contributing
1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Merge Request

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.

## 📧 Contact
Your Name - sobprom@gmail.com

Project Link: [https://gitlab.com/sobprom/deep-review-bot](https://gitlab.com/sobprom/deep-review-bot)

