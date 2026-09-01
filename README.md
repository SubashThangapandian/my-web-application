# my-web-application

A simple web application deployed using a fully automated CI/CD pipeline on AWS.

## Tech Stack
- **Source Control**: GitHub
- **CI/CD**: AWS CodePipeline
- **Build**: AWS CodeBuild
- **Hosting**: Amazon S3 (Static Website Hosting)

## Pipeline Flow
GitHub (source) → CodeBuild (build) → S3 (deploy)

Every push to the `main` branch triggers the pipeline, which builds the application and deploys it to an S3 bucket configured for static website hosting.

## Live Website
http://my-web-application-website.s3-website.ap-south-1.amazonaws.com

## Project Structure
- `index.html` - Main application file
- `buildspec.yml` - Build instructions for AWS CodeBuild