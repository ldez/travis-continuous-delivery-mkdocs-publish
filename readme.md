# Travis continuous delivery

[![Build Status](https://travis-ci.org/ldez/travis-continuous-delivery-hugo-publish.svg?branch=hugo)](https://travis-ci.org/ldez/travis-continuous-delivery-hugo-publish)

This project explains how to manipulate a Git repository within [Travis CI](https://travis-ci.org) to publish a static site on GitHub Page.


## Create mkdocs projet

```shell
mkdocs new my-folder
cd my-folder

# Display in a brawser
mkdocs serve

git init
echo "site/" > .gitignore

# Build static files
mkdocs build
mkdocs build --clean

# Deploy GitHub Pages
mkdocs gh-deploy --clean
```

## Fails

Following commands doesn't work:

```shell
git remote add docs ${GIT_REPO}
mkdocs gh-deploy -c -m $REVISION -b master -r docs
```

And fail without errors...
