GruvDoc is pre-configured [MkDocs](https://www.mkdocs.org/) project with all the must useful extensions and tweaks needed, including github workflow actions to ease the progress of deploying your docs, just Fork, Change and Push!

it tweaks [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme with [GruvBox](https://github.com/morhetz/gruvbox) color palette and uses [JetBrainsMono](https://github.com/JetBrains/JetBrainsMono) as default font.


 and start editing, then commit and push to your own repositories :)

### Usage
[Fork](https://github.com/aasmpro/gruvdoc/fork) GruvDoc github repo and Clone it or Clone the main repo:
```
git clone https://github.com/aasmpro/gruvdoc.git
```
> tip: by Forking you don't need to create and set new repo.

create a virtual environment and install packages:
```
pip install -r requirements.txt
```
serve you local version and start editing!
```
mkdocs serve
```
when you are done, commit and push changes. github actions take care of deployments.

also there is a `gitlab-ci.yml` file for GitLab users ;)

check [mkdocs-material/publishing](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more information.

### You don't want tweaks?!
you rather using GrubDoc without its tweaked theme? no problem!
just comment or delete extra css section in `mkdocs.yml` file and set your default theme!
```yaml hl_lines="4-12" linenums="87"
## Extra css files
### comment or delete these lines
### if you want to use default material theme
extra_css:
  - assets/stylesheets/fonts.css
  - assets/stylesheets/vars.css
  - assets/stylesheets/scheme.css
  - assets/stylesheets/primary.css
  - assets/stylesheets/accent.css
  - assets/stylesheets/admonitions.css
  - assets/stylesheets/utils.css
  - assets/stylesheets/styles.css
```
and comment or change:
```yaml hl_lines="9-12" linenums="11"
## Theme settings
theme:
  name: material
  favicon: assets/images/favicon.png
  features:
    - navigation.tabs
  ### comment or delete these lines
  ### if you want to use default material theme
  palette:
    scheme: gruvbox
    primary: green
    accent: green
  ### uncomment to use default material theme
  # palette:
  #   scheme: default
```
