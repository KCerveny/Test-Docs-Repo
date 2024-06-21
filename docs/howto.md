# How to Deploy MKDocs

Important Links:
- https://www.mkdocs.org/user-guide/deploying-your-docs/
- https://blog.elmah.io/deploying-a-mkdocs-documentation-site-with-github-actions/
- https://squidfunk.github.io/mkdocs-material/publishing-your-site/#with-github-actions-material-for-mkdocs
- [GitHub Action to Auto-deploy MKDocs Material](https://github.com/marketplace/actions/deploy-mkdocs)

## Standard Deployment
Following the advice given from [this](https://www.mkdocs.org/user-guide/deploying-your-docs/) tutorial. 
1. Install mkdocs, using terminal inside of VSCode
2. Initialize mkdocs repo
3. Build mkdocs, .gitignore the 'site' directory
4. mkdocs gh-deploy, put it up on repo site in under a minute

## Installing MKDocs Material
Taking the more advanced theme [Material for MKDocs](https://squidfunk.github.io/mkdocs-material/).

1. `pip install mkdocs-material`
    - Note: This needed to be run as admin on my Windows machine
2. Restart terminal in VS Code to have changes take effect
3. Run `mkdocs deploy`, changes updated shortly after 
    - Note that lots of extra folders and files will be added in to the repo under the default `gh-pages` branch

## MKDocs Material with GitHub Action
Following the CI tutorial from [MKDocs Material](https://squidfunk.github.io/mkdocs-material/publishing-your-site/#with-github-actions)

1. Create a new custom action in the documentation repository
2. Paste in the text from the above linked tutorial.
3. Commit to the main branch.