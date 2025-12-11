# TRBAM 2026 lidar bike paper presentation slides

This repo hosts the source code of the presentation slides of our lidar bike paper titled "*Quantifying Drivers-Overtaking-Bicyclists with Surrogate Safety Measures Derived from a High-Resolution Digital Lidar*".
The paper will be presented at the [Transportation Research Board Annual Meeting (TRBAM)](https://trb-annual-meeting.nationalacademies.org) 2026. 

## Basic information
- The slides are written using [Quarto presentation](https://quarto.org/docs/presentations/). The contents of the slides reside in the Quarto markdown file `index.qmd` in the `main` branch.
- The rendered slides are published with GitHub Pages using [GitHub Actions](https://quarto.org/docs/publishing/github-pages.html#github-action) specified at `.github/workflows/publish.yml`.

## For group members who are working on this slides

#### Requirements
- [Quarto](https://quarto.org/docs/get-started/)

#### How to view the slides on a local machine?
1. Clone this repository.
1. Stay on the (default) `main` branch.
1. View the slides by running `quarto preview` or `quarto render` at the root directory of the repo.

#### How to make and submit changes?

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
