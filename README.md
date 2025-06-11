# DevOps Final Project

CI/CD pipeline using GitHub Actions that:
- Dockerizes a Node.js app
- Pushes image to Docker Hub
- Deploys to AWS EC2 instance
- Auto-redeploys on push to `main`

## Secrets Required

- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`
- `EC2_HOST`
- `EC2_SSH_KEY`

## Run the App Locally

```bash
docker build -t sethsreyroth99/devops-app .
docker run -p 3000:3000 sethsreyroth99/devops-app
```

Then go to: http://localhost:3000
