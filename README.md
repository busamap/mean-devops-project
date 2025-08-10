# mean-devops-project
A simple counter app. Frontend has a button to increment a counter; clicking sends a POST to backend, which stores the count in MongoDB and returns the updated value.
mean-devops-project/
├── backend/
│   ├── Dockerfile
│   ├── server.js
│   ├── package.json
│   └── .env.example
├── frontend/
│   ├── Dockerfile
│   ├── src/ (Angular files - abbreviated)
│   ├── angular.json
│   ├── package.json
│   └── tsconfig.json
├── database/  # For MongoDB config (uses official image, but with Dockerfile for custom init)
│   └── Dockerfile
├── terraform/
│   ├── main.tf
│   ├── variables.tf
│   └── outputs.tf
├── .github/workflows/
│   ├── app-build-test.yml  # Application Pipeline
│   └── docker-build-deploy.yml  # Docker Pipeline
├── docker-compose.yml  # For local testing only
└── README.md
