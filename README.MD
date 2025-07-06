# Site Notes

## Prerequisites

- Node.js (recommend install with nvm)

## Getting started

- `npm install`

## Tooling
- `npm run build` - uses `gulp` to compile to `/dist`
- `npm run watch` - uses `gulp watch` to watch and auto-compile during development

- Right click "use live server" on `/dist/index.html` to run the site locally for development

## Deployment

- Currently I have custom domain (nikolaso.com) pointing to github.com/nosvalds/nosvalds repo, so these steps are basically to move files into `/docs` directory and then push to the `gh-pages` branch on that repo. GitHub only allow root or `/docs` directory for publishing. 

 - (one time) Set up github.com/nosvalds/nosvalds remote as a remote `git remote add git@github.com:nosvalds/nosvalds.git`)
 - Merge `main` to `gh-pages` branch
 - `npm run build` to build latest into `dist/` directory
 - `git mv dist docs` directory, or `cp -r dist/* docs/` commit
 - `git push remote gh-pages` branch
 - Then github pages will automatically publish from the `github.com/nosvalds/nosvalds` repo to www.nikolaso.com
