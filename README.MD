# Site Notes
## Tooling
`gulp` to compile to `/dist`
`gulp watch` to watch and auto-compile during development

View changes locally with `/dist/index.html`

## Deployment
```
npm run deploy
```
- This packages up /dist/ directory and pushes it to kualo hosting using the gh-pages library. 
- Kualo then auto-deploys it based on the .cpanel.yml file script


