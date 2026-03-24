# Simple Application – DevOpsSec Project

This repository contains my DevOpsSec continuous assessment project.

The application is a simple Node.js and Express app. For this project, I set up a CI/CD pipeline using GitHub Actions and deployed the app to AWS EC2. Nginx is used as a reverse proxy, PM2 is used to keep the app running, and HTTPS was enabled for secure access.

## Tools Used

- Node.js
- Express
- Git and GitHub
- GitHub Actions
- AWS EC2
- Nginx
- PM2
- DuckDNS
- Certbot / Let's Encrypt

## Live Application

[Live Site](https://devopssec-armughan.duckdns.org)

## CI/CD Overview

When code is pushed to the `main` branch, GitHub Actions runs the workflow.
The pipeline:
- checks out the code
- sets up Node.js
- installs dependencies
- runs a basic audit
- deploys the latest version to AWS EC2

## Run Locally

1. Clone the repository
2. Open the project folder
3. Install dependencies

```bash
npm install
```
Start the app in development mode

```bash
ENV=DEV npm start
```
Open in the browser:
http://localhost:8080

##Notes
This project was created for the DevOpsSec module and focuses on CI/CD, cloud deployment, and basic continuous security practices.
