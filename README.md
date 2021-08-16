
# Install Submodules

```bash
cd <project-folder-name>
git submodule init
git submodule update
```

# Testing the site

You will need to run the hugo server command with **-D** option, to show all pages & posts with **draft: true** in the front matter.

```bash
cd <project-folder-name>
hugo server -D
```

# Building the site

Building (Deployment) of the site is as follows:

- Generate static content (i.e. **public** folder) using HUGO

- Add, Commit, and Push the new static content to website repository (thus deploying the static content to the website)

- Add, Commit, and Push all configs in the project repository

## Generate static content using HUGO

Need to know the name of the template to use. (i.e. the **directory name**)

```bash
ls <project-folder-name>/themes
**NOTE DOWN THE DIRECTORY NAME OF THE THEME**
cd <project-folder-name>
hugo -t <theme-directory-name>
```

## Add, Commit, and Push the new static content to website repository

```bash
cd <project-folder-name>/public
git add .
git commit -m "Website update.."
git push
```

## Add, Commit, and Push all configs in the project repository

```bash
cd <project-folder-name>
git add .
git commit -m "Codebase of Website update.."
git push
```
