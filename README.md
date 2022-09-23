## Deploy to Netlify

Want to deploy immediately? Click this button

[![Deploy to Netlify Button](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/nuxt-toolbox)

Clicking this button will create a new repo for you that looks exactly like this one, and sets that repo up immediately for deployment on Netlify.

### Deploy using the Netlify CLI
Click the 'Use the Template' button at the top of this repo. Then install the Netlify CLI tool and run `netlify init`. Or straight from the Netlify CLI, use the `netlify sites:create-template` command in you terminal ([learn more about this command here](https://www.netlify.com/blog/create-a-site-from-a-template-using-the-netlify-cli)) to do the entire flow for you.

```bash
git clone https://github.com/netlify-templates/nuxt-toolbox 

npm install netlify-cli -g # to install the Netlify CLI tool globally

netlify init # initialize a new Netlify project & deploy
```

It will use the information from the included Netlify configuration file, [`netlify.toml`](./netlify.toml), to set up the build command as `npm run generate` to create a static project and locate the build project in the `dist` directory.

The `init` process will also set up continuous deployemnt for your project so that a new build will be triggered & deployed when you push code to the repo (you can change this from your project dashboard: Site Settings/Build & deploy/Continuous Deployment).

You can also use `netlify deploy (--prod)` to manually deploy and `netlify open` to open your project dashboard.

> 💡 we only have so many keystrokes to give, use `ntl` shorthand for `netlify` or make [an alias of your own](https://www.netlify.com/blog/2020/04/12/speed-up-productivity-with-terminal-aliases/) to save hours...of accumulated miliseconds
