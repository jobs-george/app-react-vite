# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

# Getting Started

To build a Vite project and push the build output to a different Git branch,
```sh
npm run build
```
This generates the build output in the `dist` directory.

Next, switch to a new branch,
```sh
git switch -C gh-pages
```
or
```sh
git checkout -b gh-pages
```
if the branch already exists.

Copy all of the files from the distribution folder to the root,
```sh
cp -r dist/* .
```
and commit and push to the `gh-pages` branch.