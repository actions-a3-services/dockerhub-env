# dockerhub-env/propagate

🔧 GitHub Action to propagate a Docker image to Docker Hub, including setting descriptions and categories for the Docker Hub repository, and handling Docker image build and push.

## 📌 Features

- Sets up the AMS and Docker Hub environments.
- Logs in to Docker Hub using provided credentials.
- Builds and pushes a Docker image to Docker Hub.
- Optionally updates the Docker Hub repository description and categories.
- Summarizes deployment information, including the image URL and commands for deployment.

## 🔧 Inputs

| Name        | Description                                                                    | Required | Default        |
|-------------|--------------------------------------------------------------------------------|----------|----------------|
| file        | Path to a file (`DOCKERHUB.md`) containing the full description for Docker Hub | ❓ No    | `DOCKERHUB.md` |
| username    | DockerHub username used for authentication.                                    | ✅ Yes   |                |
| token       | DockerHub access token for authentication.                                     | ✅ Yes   |                |

## 🚀 Example Usage

```yaml
- name: Propagate Docker image to Docker Hub
  uses: actions-a3-services/dockerhub-env/propagate@main
  with:
    username: ${{ secrets.DOCKERHUB_USERNAME }}
    token: ${{ secrets.DOCKERHUB_TOKEN }}
```
