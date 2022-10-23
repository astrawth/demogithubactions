# demogithubactions

Demo for Cloud computing class

## Steps for Creating Project
For each environment AWS, Azure, and GCP

- Create a Github repo

- Log into your cloud shell environment

- Create ssh key
  - ssh-keygen -t rsa
  - copy and paste key into Git SSH & GPG settings

- Clone the repo
  - git clone https://github.com/astrawth/name-of-repo
  - in this case: https://github.com/astrawth/Demo-GitHub-Actions.git
  - *copy repo name from code button*

- Create scaffold (unless you forked a project)
  - Go into your repo directory and make scaffold files
  - cd github-actions-demo/
  - touch Makefile
  - touch hello.py
  - touch test_hello.py
  - touch requirements.txt

- Create a separate environment to avoid conflicting packages
  - python3 -m venv ~/.github-actions-demo
  - source ~/.github-actions-demo/bin/activate

- Run Makefile - choose custom for each environment (AWS, Azure, GCP)
  - make install
  
 ## Steps for Creating GitHub Actions
 
 - Choose Actions in GitHub
  - Create new workflow
  - Assign name in this case I will assign it the name azure.yml
  - Copy a config or create new
  - Edit the yaml
