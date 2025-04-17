# 🛠️ Home Task 04 – CI Pipeline with GitHub Actions

This repository contains a basic **CI pipeline implementation** for a Python application using **GitHub Actions**.

## 🎯 Task Overview

The GitHub Actions workflow performs the following steps:

1. ✅ **Lint the code** using `flake8`
2. 🔐 **Login to Docker Hub**
3. 🐳 **Build and push Docker image** to Docker Hub

---

## 📁 Folder Structure

```
Home-Task-04--CI-Pipeline-with-GitHub-Actions/
│
├── Root/
│   └── app.py                # Main Python file
│
├── Dockerfile                # Docker build file
├── requirements.txt          # Python dependencies
├── .github/
│   └── workflows/
│       └── ci.yaml           # CI workflow definition
├── docs/
│   └── screenshots/
│     ├── running_workflow_pt1.png
│     ├── running_workflow_pt2.png
│     ├── running_workflow_pt3.png
│     ├── successful_workflow_pt1.png
│     └── successful_workflow_pt1.png
└── README.md
```

---

## ⚙️ CI Workflow

The CI workflow is defined in `.github/workflows/ci.yaml` and runs on every push or pull request to the `main` branch.

### 🔐 Secrets Used

Make sure the following **repository secrets** are set in GitHub:

- `DOCKER_USERNAME`
- `DOCKER_PASSWORD`

---

## 🖼️ CI Success Screenshots

### Attempts at running workflows

![running](.docs/runnning_workflow_pt1.png)
![running](.docs/runnning_workflow_pt2.png)
![running](.docs/runnning_workflow_pt3.png)

### Successful runs of workflows

![Success](.docs/successful_workflow_pt1.png)
![Success](.docs/successful_workflow_pt1.png)

---

## 🐍 Run Locally with Docker

```bash
docker build -t home-task-04 .
docker run -p 5000:5000 home-task-04
```

---

## 👨‍💻 Developed by

**Tauha Imran**  
_22i1239 DevOps Section-B_
📎 [GitHub](https://github.com/tauhaimran)
