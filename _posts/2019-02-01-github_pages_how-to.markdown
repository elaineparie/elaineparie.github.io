---
layout: post
title:      "GitHub Pages How-To "
date:       2019-02-01 20:49:23 +0000
permalink:  github_pages_how-to
---


If you’re looking for a quick (and free!) way to publish your React project, look no further than GitHub Pages. 

It’s simple, especially if you’re already working from a Github repository. 

I would first recommend installing gh-pages, which will convert your project into a publishable file. 
Run npm install gh-pages --save-dev in your terminal.  
Run npm run build
You will be prompted to add a line specifying your homepage to your package.json file (remember to replace “myname” and “myapp” with your actual specifications)
Run npm run build again. You will then be prompted to add two more lines of code to your package.json file within “scripts”:  "predeploy": "npm run build", "deploy": "gh-pages -d build"
After, run npm run deploy. This will deploy your site to the specified URL.

And boom! You are published! 

