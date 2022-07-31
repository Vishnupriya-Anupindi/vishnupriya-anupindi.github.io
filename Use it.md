# How to use this template

Working with other people's templates is always a bit annoying. 
These notes should help you to figure out where to start and how to adapt the webpage.

My guiding principle is to _keep it explicit_, instead of having tons of databases and other
fancy things everywhere.

In princple there are four tools we use:
- [Node.js](https://nodejs.org): Is used to manage the JavaScript dependencies and to run the program which generates the webpage.
- [11ty](https://www.11ty.dev/) (or eleventy.js): This is the framework which takes html-like and markdown files to generate the webpage. 
Concretely, it takes the files from `./src` and creates the webpage in `./dist`.
- [tailwindcss](https://tailwindcss.com/): A CSS framework to position elements in html. It is quite verbose and can be intimidating at first sight, but either don't use it or thrust me that this way is after a initial struggle better than alternatives.
- [alpine.js](https://alpinejs.dev/): To be honest, I don't know how it works. It's a JavaScript library to make the header menu work on smartphones 😉 

Enough theory, let's start.

## Steps

1. We need to install [Node.js](https://nodejs.org/en/download/) in your computer. 

2. Optional: I recommend to use [VS Code](https://code.visualstudio.com/) as a text editor. It has useful plugins and a useful terminal. However, in the end you just need to edit files and folders.

3. Open the root folder and run the terminal command `npm install`. This downloads all dependencies and allows you to get started.

4. Run `npm run dev`. This creates the webpage and opens a browser were you can preview the changes.
(If something does not work, use the command `npm run dev::11ty` to see the error message.)



# Setup in VS Code

The most useful parts of VS Code are probably 
the integrated terminal (to build the webpage) and the Markdown preview. 

A typical workflow would be:
- open folder
- type `npm run dev` in the terminal
- edit files
- open Markdown preview plane if wanted
- type `npm run build` and `npm run upload` to build and upload the webpage.

Optionally there are also useful extensions,
for example for better autocompletion of tailwindcss class names or the [:emojisense:]( https://marketplace.visualstudio.com/items?itemName=bierner.emojisense) extension for adding 😉 everywhere. If you want to change integral parts of how the webpage works, then extensions for Nunjucks could be useful as well.
