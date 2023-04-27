# Deploying Documentation to GitHub Pages

## Description

Create `workflow` to deploy the user `guide file` as a `Markdown` to `GitHub Pages` using a `Community Action` by converting the `Markdown` to `html` and publishing.

<!--
repoNameShort  : gihubpages-lab
repoDescription : <NONE>
 -->

## Plan

- Create plan to do as README.md file at the root directory
- The repo setting preparation
- Create basic directories and files
- Add a job to the workflow
- Check the Pages URL to confirm the Markdown has been converted to html and published.

## The repo setting preparation

In GitHub web-gui  navigate to repo.settings.pages and check next options:

- GitHub Pages / Build and deployment / Source :  [Deploy from a branch]
- GitHub Pages / Build and deployment / Branch :  [main] , [/docs]

> [main] - is branch for `Pages` - other branches will appear only after their creation
> [/docs] - is directory (folder) for `Pages`

## Create a `.github/workflows` directory and a `deploy-pages-pipeline.yaml` file  at the _root_ directory of this _repository_

```bash
mkdir -p ./.github/workflows/
touch ./.github/workflows/deploy-pages-pipeline.yaml
```

## Create a `docs` directory and a `userguide.md` file  at the _root_ directory of this _repository_

```bash
mkdir -p ./docs/
mkdir -p ./docs-src/
touch ./docs-src/userguide.md
```
