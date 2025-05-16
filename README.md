# DevOps Git Project
This task demonstrates how to manage a DevOps project using Git and GitHub, following version control best practices such as branching strategies, pull requests, tagging, and markdown documentation.

## Tools Used
- Git  
- GitHub  
- Ubuntu EC2 Instance  
- Markdown for documentation    
## Objective

The goal of this project is to simulate a real-world DevOps workflow using Git. It involves creating and managing different branches, performing pull requests, documenting tasks, and tagging versions, all while hosting the project on GitHub for collaboration and visibility.

## Project Structure

- `README.md` – Main documentation explaining the project workflow  
- `.gitignore` – File to ignore unnecessary or sensitive files  
- `Jenkinsfile` – Optional file defining a basic CI/CD pipeline  
- `feature/` – Directory or prefix for feature-specific branches  
- `screenshots/` – Folder containing Git and GitHub-related screenshots  

## Workflow Process (Step-by-Step)

### 1. Launch EC2 and Set Up Git

A new EC2 instance was created using Ubuntu, and Git was installed and configured with username and email to manage version control operations.

### 2. Initialize and Link Repository

A local Git repository was initialized and connected to a GitHub repository to allow pushing and pulling of project files and commits.

### 3. Create and Manage Branches

Three main types of branches were used:
- `main`: The production-ready branch containing the final merged code  
- `dev`: The development branch used for testing and integration  
- `feature/*`: Individual branches created from `dev` for specific features or tasks  

Each feature branch was used to isolate new work, helping ensure stability in the main codebase.

### 4. Work on Features

Files such as `.gitignore` and `Jenkinsfile` were added or modified in the feature branches. Once completed, changes were committed locally and pushed to the corresponding feature branch on GitHub.

### 5. Create Pull Requests

Pull requests were raised on GitHub to merge:
- `feature/*` into `dev` (for testing and integration)  
- `dev` into `main` (once tested and approved)  

Each pull request included a meaningful title and a description explaining the purpose of the changes.

### 6. Add Version Tags

Once development was complete and changes were merged into the `main` branch, a version tag (such as `v1.0`) was created to mark the release point of the project.

## Screenshots

Screenshots were captured and saved in the `screenshots/` folder. These include:
- Git configuration in the EC2 instance  
- Branch creation and switching  
- Commit logs and pull request pages on GitHub  
- Tag creation and repository status  
- Jenkinsfile view (if included)  

## Outcome

- Successfully implemented a version-controlled DevOps project using Git and GitHub  
- Followed a complete Git lifecycle from branching to merging and tagging  
- Practiced clean collaboration practices through pull requests  
- Demonstrated readiness for real-world DevOps workflows  
- Maintained a well-structured and documented Git repository  


