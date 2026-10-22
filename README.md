# AWS DevOps Portfolio Project

## About
A simple portfolio website built with HTML and CSS, containerized using Docker, and hosted using GitHub Pages.

## Technologies Used
- HTML and CSS
- Git and GitHub
- Docker
- Nginx
- GitHub Actions
- Docker Health Checks

## What I Learned
- Created and hosted a website using GitHub Pages.
- Built a Docker image using a Dockerfile.
- Ran the website inside a Docker container.
- Created a CI workflow using GitHub Actions.
- Automated Docker image builds on every push.
- Configured a Docker health check to monitor container health.
- Practised checking container status, logs, CPU, and memory usage.

## How to Run
1. Clone this repository.
2. Build the Docker image:

   ```bash
   docker build -t my-portfolio .
   ```

3. Run the container:

   ```bash
   docker run -d -p 8080:80 --name my-portfolio-container my-portfolio
   ```

4. Open http://localhost:8080 in your browser.
5. Check container health:

   ```bash
   docker ps
   ```

   Look for `healthy` in the STATUS column.

## Project Workflow
Developer → GitHub → GitHub Actions → Website checks → Docker image build

## Architecture
- **Source Code:** GitHub repository
- **CI Automation:** GitHub Actions
- **Containerization:** Docker
- **Web Server:** Nginx
- **Website Hosting:** GitHub Pages
- **Local Container URL:** http://localhost:8080

## Future Improvements
- Deploy the container to AWS.
- Add more automated tests.
- Learn AWS networking and IAM.
- Extend the CI/CD pipeline to automate deployment.

## Author
Ajayraje Patil
