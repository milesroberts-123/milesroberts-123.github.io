
My website is built with [mkdocs.org](https://mkdocs.org) and hosted on [github pages](https://pages.github.com/).

This page documents the process of me learning how to build a website with these tools. I'm probably the only one that will find it interesting, but I'll make it public just for fun!

# mkdocs Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

# Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

# Editing the website

```
# build website from markdown files in docs/
mkdocs build

# copy output of mkdocs to top level of repo, necessary for github pages to work
cp -r site/* .; rm -r site/

# stage changes, add commit message, push to github pages repo
git add --all

git commit -m "Any note I want"

git push -u origin master
```

Then enter the personal access key twice. Generate keys via: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

# Helpful resources for building websites from scratch

[Quick tutorial on HTML and CSS](https://happycoding.io/tutorials/html/html)

[HTML reference](https://www.w3schools.com/TAgs/default.asp)

[CSS reference](https://www.w3schools.com/css/default.asp)

[Change website domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)
