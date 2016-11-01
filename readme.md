
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

DOESN'T WORK :'(

```shell
git remote add docs ${GIT_REPO}
mkdocs gh-deploy -c -m $REVISION -b master -r docs
```

Fail without errors...
