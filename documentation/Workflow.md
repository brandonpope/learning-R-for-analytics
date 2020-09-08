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
  - Roger Dudler's [git - the simple guide](https://rogerdudler.github.io/git-guide/)
  - [Azure Dev Ops Git Repos tutorial](https://docs.microsoft.com/en-us/azure/devops/repos/git/gitworkflow?view=azure-devops)
  - Depending on the size of your team/repository, and the complexity/maturity of your software development evironment, branch/release/deployment can get way more complicated than this docuent is meant to address
  - For getting started - I recommend the following workflow. This workflow is written to be executed from the command line, but could similarly be partially/completely executed from a web GUI (Azure DevOps, GitHub...):
    1. Clone your repository by copying the url
    ```
    $ git clone <repository_url>
    ```
    2. Create a branch and check it out - choose a branch name related to the features/fix/development you are working on
    ```
    $ git checkout -b <branch_name>
    ```
    3. Make changes to the code as desired and save files
    4. Commit the changes to the branch
    ```
    $ git add .
    $ git commit -m "comment describing your change"
    ```
    5. Switch back to the `master` branch
    ```
    $ git checkout master
    ```
    6. Push the changed branch to the origin
    ```
    $ git push origin <branch_name>
    ```
    7. Create a pull request to merge `<branch_name>` with `master`
    8. Review and (when appropriate) approve the pull request (and delete `<branch_name>`)
    9. On your local machine, update `master`
    ```
    $ git pull origin master
    ```
- [Here](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf) is a Git cheatsheet from GitHub

## Reproducible Analyses

- Anna Krystalli's [Reproducible Research Data & Project Management in R](https://annakrystalli.me/rrresearchACCE20/)
- Software Carpentry's [R for Reproducible Scientific Analysis](http://swcarpentry.github.io/r-novice-gapminder/)
- Dean Marchiori's [The meta-concepts of data analysis, workflows and projects in R](https://github.com/deanmarchiori/analysis-flow)

## Other Resources
- Jim Savage's [agile and testing thoughts](https://threader.app/thread/1136987234362691585)
