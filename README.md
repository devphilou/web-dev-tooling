# (web) dev-tooling
Default tooling setup like formatters etc

#### Editor
1. [Visual Studio Code](https://code.visualstudio.com/)
    * Install [Prettier](https://prettier.io/) Extension
        * Format on save: File > Preferences > Settings > search "format on save" > tick "Editor: Format On Save"
        * Use [prettier config](https://github.com/devphilou/web-dev-tooling/blob/main/.prettierrc)
     * Integrate [Linter with Prettier](https://prettier.io/docs/en/integrating-with-linters.html)
         * [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
     * Install [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons) or [material icon theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
     * Install [Gitlens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
     * Install [GitHistory](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory)
     * Install [GitGraph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
     * Install [IntelliJ Keybindings](https://marketplace.visualstudio.com/items?itemName=k--kato.intellij-idea-keybindings)
     * Install [Rainbow Brackets](https://marketplace.visualstudio.com/items?itemName=2gua.rainbow-brackets)
     * Install [Auto-Rename-Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
     * Install [Javascript Snippets](https://marketplace.visualstudio.com/items?itemName=xabikos.JavaScriptSnippets)
     * Install [HTML Snippets](https://marketplace.visualstudio.com/items?itemName=abusaidm.html-snippets)
     * Install [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
     * Install [Import Cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
     * Install [SVG](https://marketplace.visualstudio.com/items?itemName=jock.svg)
     * Install [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client)
     * Install [TODO Highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight)
     * Helpful
         * [Draw.io Integration](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)
         * [Tailwind Intellisense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss)
         * [Angular Snippets](https://marketplace.visualstudio.com/items?itemName=johnpapa.Angular2)
         * [Angular Language Service](https://marketplace.visualstudio.com/items?itemName=Angular.ng-template)
         * [React Snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
         * [NodeJs Extension Pack](https://marketplace.visualstudio.com/items?itemName=waderyan.nodejs-extension-pack)
         * [NestJS Snippets](https://marketplace.visualstudio.com/items?itemName=ashinzekene.nestjs)
         * [Node Snippets](https://marketplace.visualstudio.com/items?itemName=chris-noring.node-snippets)

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

## Other

#### MacOS
   * [Homebrew](https://brew.sh/index_de)
   * `brew install nvm` -> `nvm install --lts`
   * `brew install jenv`
      * `echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.zshrc`
      * `echo 'eval "$(jenv init -)"' >> ~/.zshrc`
   * Java
      * `brew install maven` (will also install current java)
         * `jenv add /opt/homebrew/Cellar/openjdk/17.0.1_1/libexec/openjdk.jdk/Contents/Home`
      * Install [SDKMan](https://sdkman.io/install)
      * `sdk list java` -> install e.g. JAVA 8 with `sdk install java 8.0.312-zulu`
         * `jenv add ~/.sdkman/candidates/java/current/zulu-8.jdk/Contents/Home`
      * `jenv versions` -> `jenv global 1.8`
      * `sdk install gradle`

#### OS (Ubuntu)
* Install wifi usb driver: https://github.com/aircrack-ng/rtl8812au
   * `sudo apt update && sudo apt install build-essential git dkms`
   * `git clone https://github.com/aircrack-ng/rtl8812au`
   * `cd rtl8812au`
   * `sudo make dkms_install`
