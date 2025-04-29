# dockerhub-env/get

🔧 GitHub Action to download and set Docker Hub environment variables, and optionally display them in a step summary.

## 📌 Features

- Downloads Docker Hub environment variables from an artifact.
- Sets Docker Hub environment variables for the current GitHub Actions run.
- Optionally generates a summary of Docker Hub environment variables and appends it to the GitHub Actions step summary.

## 🔧 Inputs

| Name     | Description                                  | Required | Default |
|----------|----------------------------------------------|----------|---------|
| summary  | Enable or disable the summary output         | ❓ No    | `false` |

## 🚀 Example Usage

```yaml
- name: Get Docker Hub environment variables
  uses: actions-a3-services/dockerhub-env/get@main
  with:
    summary: 'true'
```
