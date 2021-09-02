---
hide:
  - navigation
---
GruvDoc is pre-configured [MkDocs](https://www.mkdocs.org/) project with all the must useful extensions and tweaks needed, just Fork, Change and Push!

### Features
- GruvDoc is all extra config files, anything can be [changed](#you-dont-want-tweaks) easily.
- Tweaks [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) under the hood!
- [GruvBox](/gruvdoc/docs/colors/) color palette with 24 different colors for both primary and accent.
- [JetBrainsMono](/gruvdoc/docs/fonts/) font.
- Simple, pre-configured [mkdocs.yml](https://github.com/aasmpro/gruvdoc/blob/master/mkdocs.yml) file.
- [Github](https://github.com/aasmpro/gruvdoc/blob/master/.github/workflows/gruvdoc.yml) / [Gitlab](https://github.com/aasmpro/gruvdoc/blob/master/.gitlab-ci.yml) Workflows included for auto Deployment!
- Including [Styles](/gruvdoc/docs/styles/) and custom [Utils](/gruvdoc/docs/utils/).

### Usage
[Fork](https://github.com/aasmpro/gruvdoc/fork) GruvDoc github repo and Clone it or Clone the main repo:
```
git clone https://github.com/aasmpro/gruvdoc.git
```
!!! quote "by [Forking](https://github.com/aasmpro/gruvdoc/fork) you don't need to create and set new repo."

create a virtual environment and install packages:
```
pip install -r requirements/gruvdoc.txt
```
serve your local version and start editing!
```
mkdocs serve
```
when you are done, commit and push changes. workflows will take care of deployments.

check [mkdocs-material/publishing](https://squidfunk.github.io/mkdocs-material/publishing-your-site/) for more information.

#### In another repo
if you want to add GruvDoc in another project:

- copy `docs` folder to your project
- copy `mkdocs.yml` file to your project
- copy `requirements` folder to your project
- copy `.github/workflows/gruvdoc.yml` or `.gitlab-ci.yml` for workflows
 

### You don't want tweaks?!
you rather using GrubDoc without its tweaked theme? no problem!
just comment extra css section in `mkdocs.yml` file:
```yaml hl_lines="4-12"
## Extra css files
### comment these lines,
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
and then set your palette:
```yaml hl_lines="6-9"
## Theme settings
theme:
  name: material
  ### comment these lines,
  ### if you want to use default material theme
  palette:
    scheme: gruvbox
    primary: green
    accent: green
  ### uncomment to use default material theme
  # palette:
  #   scheme: default
```
you can change anything by editing only `mkdocs.yml` file.
