# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

# Getting Started

Ensure that your `vite.config.js` file includes the correct `base` property. 
This property should be set to the name of your repository. 
For example:
```javascript
import { defineConfig } from 'vite';
import react from '@vitejs/plugin-react';

export default defineConfig({
    base: '/your-repo-name/',
    plugins: [react()],
});
```
Run the build command to generate the production files:
```sh
npm run build
```
You can use the `gh-pages` package to deploy your build output to GitHub Pages. 

First, install the package:
```sh
npm install gh-pages --save-dev
```
Then, add the following scripts to your `package.json`:
```json
"scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
}
```
Finally, deploy your project:
```sh
npm run deploy
```
Make sure that GitHub Pages is set to serve from the `gh-pages` branch in your repository settings.