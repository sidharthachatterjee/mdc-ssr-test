# mdc-ssr-test

Reproduces a bug in [material-components-web-react](https://github.com/material-components/material-components-web-react) where SSR for Button fails due to usage of HTMLElement

Breaks with 
```
if (matchesMethod in HTMLElementPrototype) {
                      ^
TypeError: Cannot use 'in' operator to search for 'matches' in undefined
```
