# Jenkins Practice Projects

A set of Jenkins exercises, from installing Jenkins to building multi-stage pipelines
with Docker, shared libraries and webhooks. The folders are numbered in the order I
worked through them. Each folder has its own README with the steps and notes.

## Folders

| Folder | Topic |
|--------|-------|
| `1-installation` | Installing Jenkins |
| `2-Jenkins-pipeline` | Scripted and declarative pipeline syntax, with a small Java example (`First.java`) |
| `3-java-jenkins-docker-app` | Maven Java app: build, test and Docker image pipeline (`Jenkinsfile`, `Dockerfile`, `docker-compose.yml`) |
| `4-python-jenkins-docker-app` | Python app: install, test and Docker image pipeline (`app.py`, `tests/`, `Dockerfile`) |
| `5-Agent-Setup` | Setting up a Jenkins build agent (`jenkins-agent-init-run`) |
| `6-Agent-execution` | Running a pipeline on an agent (`python-app`) |
| `7-Environment-Variables` | Environment variables and credentials in a pipeline |
| `8-Project-1-Python-Flask-App` | Project: Flask app pipeline |
| `9-Project-2-React-github-summarizer` | Project: React app pipeline |
| `10-Project-3-maven-jenkins-cicd` | Project: Maven CI/CD pipeline |
| `11-github-webhook` | Triggering builds from GitHub webhooks |
| `12-jenkins-shared-library` | Jenkins shared libraries |

## Running the examples

Each example needs Jenkins with the Pipeline plugin, and most need Docker and Maven
or Python on the agent. Start with the folder that matches the step you are on, then
read its README for the exact setup.

## Notes

- Some folders are still notes or stubs, with a README only. Check the folder before relying on it.
- Build output (`target/`) and `.DS_Store` files are excluded in `.gitignore`.
