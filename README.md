# Streamline CV

This tools helps you to deal with CV and cover letter routine.

## Quickstart

1. Create a repository from this template, make sure you make it **private**.
2. Change something in `config.yaml`, just a dry run for the beginning.
3. On commit to `main` CI will start and create a new release that includes your CV and cover letter as artifacts.

It's that straightforward!

## Branch/PR workflow

Branch and PR is a more
flexible [workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow).

1. Create a branch and fill `config.yaml` with your CV and cover letter data.
2. Create a PR in GitHub.
3. CI will do the rest for you
    * Build PDF for a CV and a cover letter and provide as a link to download.
    * Suggest improvements via AI.
    * ...

This is handy when you need to have parallel versions of CV and cover letter, you could actually never merge them to
main.

## Hot it works?

This project assembles several tools into a ready-to-go solution with a very low entry level.

### GIT

Git tracks changes and does version management of your CV.

### GitHub

GitHub provides a lot of useful features on top of Git, such as:

- Pull requests for clear changes navigation.
- CI for heavy work so that you don't need to set up tools locally.
- Edit CV easily
    - Edit via GitHub UI or Codespaces
    - Use copilot right there if you have it!
    - Edit locally in your favourite IDE

### CV and cover letter rendering

It uses [rendercv](https://github.com/achugr/rendercvcl) tool
that takes yaml configuration file and renders it as a fancy pdf.
The tool is wrapped into GitHub action that does all the work in the CI and puts a comment with a link for download.
