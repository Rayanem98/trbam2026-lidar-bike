# The source code of the lidar bike slide presentation at the TRBAM (Transportation Research Board Annual Meeting) 2026

## Basic setup
- The slides' contents are written in Markdown in the Quarto markdown file `index.qmd`. More information on the Quarto presentation can be [found here](https://quarto.org/docs/presentations/).
- The rendered slides are published with GitHub Pages using [GitHub Action](https://quarto.org/docs/publishing/github-pages.html#github-action) specified at `.github/workflows/publish.yml`.

## How to collaborate?

### Requirements
- [Quarto](https://quarto.org/docs/get-started/)

### How to view the slides on a local machine?
1. Clone the repository.
1. View the slides by running `quarto preview` or `quarto render` at the root directory of the repo (at the default `main` branch).

### How to make and submit changes?

Changes should be submitted via GitHub Pull Requests (PRs).

1. Create and switch to a new branch for your task. Name it after what you plan to do. For example,
    ```{shell}
    git switch -c add-intro-slide
    ```
1. Make changes by editing files. Test locally with `quarto preview` or `quarto render`.
1. Keep in mind that the remote `main` branch might change after you cloned the project. Keep your task branch updated while you are working on your task.
    ```{shell}
    git switch main
    git pull
    git switch add-intro-slide
    git merge main
    ```
1. Commit your changes and push the branch to GitHub.
1. Open an PR on GitHub.
1. After the PR is merged, clean up locally by deleting the branch.
    ```{shell}
    git switch main
    git pull origin main
    git branch -d add-intro-slide
    ```
