# Heroku
The case of usage is simple: You have built an app with your favorite front picture, you want it to be checked and seen with your users without having to think about technicalities. Heroku will support your app directly in seven steps from your remote repository.

1. Create the App on Heroku
Before you get started, make sure everything is pushed to your GitHub or other remote repo

- Run the command:

This will create your app on Heroku (which makes Heroku accessible to you) and create two links:

```
Creating app... done, ⬢ fakestuff-farboo-84560
https://fakestuff-farboo-84560.herokuapp.com/ | https://git.heroku.com/fakestuff-farboo-84560.git
```

2. Set the Node Server Configuration
`$ heroku config:set NPM_CONFIG_PRODUCTION=false`

This command informs Heroku to install devDependencies. More specifically, this overwrites the cutting stage and accesses packages declared during execution under devDependencies. This helps Heroku to start developing npm run.

3. Listen to the Host 0.0.0.0
`$ heroku config:set HOST=0.0.0.0`

4. Run Node in Production Mode
`$ heroku config:set NODE_ENV=production`

5. Tell Heroku to Run “npm run build"

Then, in our package.json format, we need to add a script to tell Heroku to run NPM create. Only add a "heroku-postbuild":"npm run build" line to your "script" object.json

```
"scripts": {
  "dev": "nuxt",
  "build": "nuxt build",
  "start": "nuxt start",
  "generate": "nuxt generate",
  "lint": "eslint --ext .js,.vue --ignore-path .gitignore .",
  "heroku-postbuild": "npm run build"
}
```
6. Create a Procfile for Heroku
To run and execute our program, Heroku requires a profile. We just have an extension at the root of our application folder to create a tab, call it Profile, and add the following line inside.

`web: npm run start`

Start NPM run is the application fired script that is guided to HTTP traffic by the web.

7. Push Your GitHub Repo to Heroku to Deploy

Finally, all you have to do is ACP  our configured app.
