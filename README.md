
[![Demo Python Application test with Github Actions](https://github.com/astrawth/demogithubactions/actions/workflows/main.yml/badge.svg)](https://github.com/astrawth/demogithubactions/actions/workflows/main.yml)# demogithubactions

[Loom Video of CI Demo](https://www.loom.com/share/581af99f85ce4035bdb4f45979057873)

Demo for Cloud computing class

## Steps for Creating Project

- Create a Github repo

- Log into your cloud shell environment

- Create ssh key
  - ssh-keygen -t rsa
  - copy and paste key into Git SSH & GPG settings

- Clone the repo
  - git clone https://github.com/astrawth/name-of-repo
  - in this case: https://github.com/astrawth/demogithubactions.git
  - *copy repo name from code button*

- Create scaffold (unless you forked a project)
  - Go into your repo directory and make scaffold files
  - cd github-actions-demo/
  - touch Makefile
  - touch hello.py
  - touch test_hello.py
  - touch requirements.txt

- Create a virtual environment to avoid conflicting packages
  - python3 -m venv ~/.demogithubactions
  - source ~/.demogithubactions/bin/activate

- Run Makefile - choose custom for each environment (AWS, Azure, GCP)
  - make install
  - make lint
  - make test
  - make format
  - or you can add a all: intstall lint test
  
 ## Steps for Creating GitHub Actions
 
 - Choose Actions in GitHub
  - Create new workflow
  - Name your workflow
  - Edit the main.yml (copy a template or create new)
  - select your workflow to review the build for success
  - If successfully you can copy the badge and paste in your readme


