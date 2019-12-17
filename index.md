# Learn to build a nuxt js app

## install node.js
> on windows platform, just download the latest LTS version and install, the installer will take care of the previous installed version if any. So don't worry about the upgrade issue.

## create nuxt project
1. `npx creat-nuxt-app *project-name*`  
2. select Element as UI framework
3. select axios
4. select Eslint, Prettier
5. select Jest
6. select Universal(SSR)

## install vscode and extensions below as a start
1. HTML Snippets
2. Material Icon Theme
3. Monokai
4. Vetur
> The extension list will grow along progress

## start the scaffolding app
1. `npm run dev`
2. open web browser and navigate to the development server <localhost:3000>

## check element-ui availability
1. Delete the index.vue template
2. Add some element-ui component to see if it effects

## add admin page
1. Add admin.vue in the pages folder
2. Add `<h1>This is admin page</h1>`
3. Navigate to <localhost:3000/admin> and see if the route works automatically

## add programmatic navigation between home page and admin page
1. add links in home and admin pages
2. use `this.$route.push('*path*')` in the click handler

## eslint problem
> Disable eslint for a block of codes
`/* eslint-disable */`  
`*some lines of code*`  
`/* eslint-enable */`

> By using `npm run lint -- --fix`, some eslint errors/warnings can be fixed automatically

## prettier problem
1. install prettier vscode extension
2. add `"endOfLine": "auto"` in project .prettierrc file
3. Choose prettier as document formatter (described in the articles below)
4. Turn on "format on save" in workspace settings
5. See articles <https://scotch.io/tutorials/code-formatting-with-prettier-in-visual-studio-code> and <https://glebbahmutov.com/blog/configure-prettier-in-vscode/>
in short, add following in workspace settings.json,
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true
}
