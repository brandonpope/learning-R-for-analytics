# Workflow

## Version Control

- Version control is something that I still don't have good habits/maturity around, but is really important to scale analytics efforts well (in time, team, complexity...).

### Git/GitHub

- [GitHub](www.github.com) is a popular collaboration and version control host for coding and software development, there are a lot of resources online about GitHub, e.g. [GitHub Guides](https://guides.github.com/).
- GitHub workflow can get intricate in mature production software environments, again I'm not a software developer, but there are several very important tools that GitHub facilitates well:
  - Pull requests to support peer review of proposed changes to code
  - Diffable code identification and highlighting, reviewers, commenting... to support peer review
  - Change and history tracking and reversion capabilities
  - Distributed contribution
  - Issue creation
  - Transparency and discoverability through a centralized repository of production code
- For basic GitHub workflows, see:
  - [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
  - [Azure Dev Ops Git Repos tutorial](https://docs.microsoft.com/en-us/azure/devops/repos/git/gitworkflow?view=azure-devops)
  - For getting started - I recommend the following workflow:
    1. Clone your repository
    ```
    git clone <repository_url>
    ```
    2. Create a branch and check it out
    ```
    git checkout -b <branch_name>
    ```
    3. Make changes to the code as desired
    4. Commit the changes to the branch
    ```
    $ git add .
    $ git commit -m "comment describing your change"
    ```
- [Here](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf) is a Git cheatsheet from GitHub
  
## Resources
- Jim Savage's [agile and testing thoughts](https://threader.app/thread/1136987234362691585)
