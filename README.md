# [MumPy Website](#)
>
> Theme taken from [mkdocs-simple-blog](https://github.com/FernandoCelmer/mkdocs-simple-blog)

<!-- ![Image](https://raw.githubusercontent.com/FernandoCelmer/mkdocs-simple-blog/develop/docs/assets/simple-blog.png) -->

<!-- ![GitHub forks](https://img.shields.io/github/forks/FernandoCelmer/mkdocs-simple-blog?label=Forks&style=flat-square)
![GitHub Repo stars](https://img.shields.io/github/stars/FernandoCelmer/mkdocs-simple-blog?label=Stars&style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/FernandoCelmer/mkdocs-simple-blog?style=flat-square)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/FernandoCelmer/mkdocs-simple-blog/python-publish-pypi.yml?label=%F0%9F%93%A6%20PyPI&style=flat-square)
![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/FernandoCelmer/mkdocs-simple-blog/python-publish-pypi-test.yml?label=%F0%9F%93%A6%20PyPI-Test&style=flat-square) -->

## Install

### Installation MkDocs

To install MkDocs, run the following command from the command line:

```bash
pip install mkdocs
```

### Installation theme

Install the theme using PIP:

```bash
pip install mkdocs-simple-blog
```

### Preview/ Run Locally

```bash
mkdocs serve
```

### Build and deploy to gh pages

1. commit and push all the changes to `main` branch

```bash
git add . && git commit -m "your commit message"
git push origin main
```

2. Checkout/switch to the `gh-pages` branch and rebase with the latest changes of the main branch

```bash
git switch gh-pages && git rebase origin/main
```

3. Build your MkDocs site using `mkdocs build` command

4. Navigate to the `/site` directory in your local repository and create a temporary git repository:

```bash
cd site
git init
```

5. Commit the Changes & push to `gh-pages` branch:

```bash
git add . && git commit -m "Deploy MkDocs Site"
git push -f https://github.com/mumbaipy/website.git master:gh-pages
```

6. Clean up:

Once you've successfully pushed to gh-pages, you can delete the temporary Git repository in the /site directory:

```bash
rm -rf .git
```

## Need Help?

Read the MkDocs [Documentation](https://www.mkdocs.org/getting-started/) :)

## License

![GitHub](https://img.shields.io/github/license/FernandoCelmer/mkdocs-simple-blog?style=flat-square)

This project is licensed under the terms of the MIT license.
