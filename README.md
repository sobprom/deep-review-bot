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
