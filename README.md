# gitHub-pages-deployments

*GitHub Pages Deployment Workflow*
Project Page: https://roadmap.sh/projects/github-actions-deployment-workflow

This repository contains a GitHub Actions workflow to automate the deployment of a static website to GitHub Pages. The workflow is designed to simplify the process of publishing your site by automatically deploying new changes whenever you push to the main branch.

How It Works
The workflow is defined in .github/workflows/deploy.yml. Upon every push to the main branch, the workflow will:

Checkout the code: It gets the latest version of your repository.

Deploy to GitHub Pages: It uses the peaceiris/actions-gh-pages action to take the contents of the public directory and push them to a gh-pages branch. This is the branch that GitHub Pages uses to serve your live website.

Prerequisites
A GitHub repository with a public directory containing your static website files (e.g., index.html, style.css, etc.).

The workflow file saved at .github/workflows/deploy.yml.

Deployment
To deploy your website, simply push your changes to the main branch of your repository. The GitHub Actions workflow will handle the rest.

git add .
git commit -m "feat: Add new website content"
git push origin main

