# web-dev-tooling
Default tooling setup like formatters etc

#### Editor
1. [Visual Studio Code](https://code.visualstudio.com/)
    * Install [Prettier](https://prettier.io/) Extension
        * Format on save: File > Preferences > Settings > search "format on save" > tick "Editor: Format On Save"
        * Use [prettier config](https://github.com/devphilou/web-dev-tooling/blob/main/.prettierrc)
     * Integrate [Linter with Prettier](https://prettier.io/docs/en/integrating-with-linters.html)
     * Install [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons)

#### CLI
2. Optional: install zsh `apt get install zsh`
3. [OhMyZsh](https://ohmyz.sh/#install)
4. Edit `vim .zshrc`
    * `ZSH_THEME=crcandy`
    * `alias gst="git status"`
    * `alias go="git checkout"`
    * `alias got="git checkout --track"`
    * `alias gis="git stash"`
    * `alias gsp="git stash pop"`
    * `alias gsl="git stash list"`

#### Node
5. Install [Node Version Manager](https://github.com/nvm-sh/nvm)
    * `nvm install --lts`

#### Bundler
6. [Webpack](https://webpack.js.org/)
7. [Parcel](https://parceljs.org/)
    * `npm install -g parcel-bundler`
