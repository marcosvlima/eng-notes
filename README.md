# Eng Notes

Engineering Notes and Troubleshooting Guide

Build with:

- mkdocs
- mkdocs-material

## Start development server
```
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

## Build documentation
```
docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material build
```

## Deploy documentation to GitHub Pages
```
docker run --rm -it -v ~/.ssh:/root/.ssh -v ${PWD}:/docs squidfunk/mkdocs-material gh-deploy 
```

For detailed installation instructions, configuration options, and a demo, visit squidfunk.github.io/mkdocs-material