# Project Setup Automation

These are the tasks we need to do:

- Clone this project to the current folder: {CLONE_URL}
- Install dependencies
- Init Local Git (if not already present)
- Programmatically Create a Remote Repository on GitHub, with name: {REMOTE_NAME}
- Push Local Changes to the New GitHub Remote
- Create a Vercel Project and Setup CI/CD Pipeline, with the Vercel CLI.

Configure the CI/CD pipeline so that any commits to the remote GitHub trigger a deployment on Vercel.

vercel login --token {VERCEL_TOKEN}  # if not already authenticated

vercel init   # initialize a Vercel project if needed

vercel link   # link the project to your personal GitHub repo

- Analyze the Code to Auto-Generate Developer Guidelines (.cursorrules)

Analyze the repository's code to extract conventions such as coding style, file structure, naming conventions, commit message patterns, etc.

Generate a Developer Guidelines file named .cursorrules that documents these conventions.
 
- Generate a GitHub Pull Request Template
Create a GitHub pull request template to guide contributors when submitting pull requests.
This file should be placed in the `.github` directory as `PULL_REQUEST_TEMPLATE.md`.

- Make CursorPROMPT.md file and add this prompt to the file. But replace tokens and URL's with placehoders

- Commit and Push all changes
Add the newly created .cursorrules file to the Git repository.
Commit and push the file to the remote GitHub repository.

----------------
RemoteName: {REMOTE_NAME}
CloneURL: {CLONE_URL}
Github PAT: {GITHUB_PAT}
Github Account: {GITHUB_ACCOUNT}
VercelToken: {VERCEL_TOKEN} 