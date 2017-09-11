# README
`static-template` is a frontend template for quick and easy development of a simple static website ready to be deployed to Netlify.

The `master` branch contains the most basic version of the template. The other branches in the repo offer variations on the template with a more opinionated approach to the code structure, frameworks, etc.

## Development
* `npm i` to install development dependencies
* `npm run build` to create a development ready build located in the `build` folder
* `npm run start` to start a development server and watch for changes within the `build` folder
* `npm run deploy` to create a production ready build located in the `dist` folder

## File Structure
```
├── src
│   ├── index.html              # Static HTML file
│   ├── img/                    # Contains all images used on the website
│   ├── js/                     # Contains all Javascript/Component files to be compiled
│   │    └──scripts.js          # Javascript entry point (ES6 compatible via Babel)
│   └── scss/                   # Contains all styling to be compiled
│        └──style.scss          # Sass entry point
|
└── build                       # Generated build folder created via npm run build
└── dist                        # Generated dist folder created via npm run deploy
```

## Deploy to Netlify
1. Sign up for a [Netlify account](https://app.netlify.com/signup)

2. Follow the [documentation](https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/) to connect to a Git provider and select the desired repository to be deployed.

3. On the final step configure your site with the following build settings:
* Build command: `npm run deploy`
* Publish directory: `dist`
