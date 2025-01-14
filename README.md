```txt
******** **      **   ******
/**///// /**     /**  **////**
/**      /**     /** **    //
/******* //**    ** /**
/**////   //**  **  /**
/**        //****   //**    **
/**         //**     //******
//           //       //////

+-+-+-+-+-+-+-+-+
|D|o|t|f|i|l|e|s|
+-+-+-+-+-+-+-+-+
```

# Dotfiles

[![GitHub Issues](https://img.shields.io/github/issues/FrancesCoronel/dotfiles.svg?style=flat-square)](https://github.com/FrancesCoronel/dotfiles/issues) [![GitHub Pull Requests](https://img.shields.io/github/issues-pr/FrancesCoronel/dotfiles.svg?style=flat-square)](https://github.com/FrancesCoronel/dotfiles/pulls) [![MIT License](https://img.shields.io/github/license/FrancesCoronel/dotfiles.svg?style=flat-square)](http://badges.mit-license.org)

> This sets up my dev environment to be very Material Design friendly.
>
> Background photo from [Unsplash Wallpaperss](https://unsplash.com/).

![Showcase](https://i.imgur.com/ErIiC3v.png)

- [Installation](#installation)
  - [Alfred](#alfred)
  - [Chrome](#chrome)
    - [Chrome Extensions](#chrome-extensions)
  - [Desktop](#desktop)
  - [Fonts](#fonts)
  - [Visual Studio Code Editor](#visual-studio-code-editor)
    - [Open with Terminal](#open-with-terminal)
    - [Visual Studio Code Extensions](#visual-studio-code-extensions)
  - [Homebrew](#homebrew)
  - [macOS Apps](#macos-apps)
    - [Casks](#casks)
    - [Manual](#manual)
    - [Menubar](#menubar)
  - [Screensaver](#screensaver)
  - [Shells](#shells)
    - [Hyper](#hyper)
    - [iTerm 2](#iterm-2)
    - [Terminal](#terminal)
  - [Tracking](#tracking)
- [Theming](#theming)
- [Usage](#usage)
- [Contributing](#contributing)
  - [Code of Conduct](#code-of-conduct)
- [Credits](#credits)
  - [Kudos](#kudos)

## Installation

The `sudo` command is necessary for Homebrew to be installed and for some others.

```bash
# Download latest version from Github
curl -L -O https://github.com/FrancesCoronel/dotfiles/archive/7.0.zip

# Unzip the file and move to root
unzip 7.0.zip && mv dotfiles-7.0 .dotfiles && rm 7.0.zip

# Run bootstrap!
sh ~/.dotfiles/bootstrap.sh

# Installs npm and certain npm packages
sh ~/.dotfiles/init/.npm

# Installs casks and taps to caskroom-versions
sh ~/.dotfiles/init/.casks

# Installs oh-my-zsh, terminal theme, oh-my-zsh theme and configs
sh ~/.dotfiles/init/.shell

# Installs optimal macOS system settings
sh ~/.dotfiles/init/.osx

# Installs fonts for coding and docs
sh ~/.dotfiles/init/.fonts

# Setups git configuration settings
sh ~/.dotfiles/init/.gituser
```

### Alfred

With Alfred, I use a theme called [Materialize](https://www.alfredapp.com/extras/theme/5hT6cEQ6h1/) that is published online for anyone to install through Alfred Themes.

### Chrome

I use a basic white theme for Chrome.

![Chrome Theme](https://i.imgur.com/qZjkvIo.png)

#### Chrome Extensions

- 1Password – Password ManagerAdGuard AdBlocker
- Application Launcher For Drive (by Google)
- Awesome Screenshot and Screen Recorder
- axe DevTools - Web Accessibility Testing
- Calendly: Meeting Scheduling Software
- Clockwise: Team Time & Calendar Management
- Designer Tools
- GIFs for GitHub
- GoFullPage - Full Page Screen Capture
- Google Docs Offline
- Grammarly: Grammar Checker and Writing App
- I'm a Gentleman
- JSONVue
- Loom – Free Screen Recorder & Screen Capture
- Material Icons for GitHub
- Neutral Face Emoji Tools
- Notifier for GitHub
- Notion Web Clipper
- Office Editing for Docs, Sheets & Slides
- Page Ruler
- Panda 5 - Your favorite websites in one place
- Pushbullet
- Raindrop.io
- React Developer Tools
- Refined GitHub
- Sprucemarks
- Todoist for Chrome
- Todoist for Gmail
- Todoist New Tab
- WakaTime
- Wappalyzer - Technology profiler
- Wikiwand: Wikipedia Modernized

### Desktop

I use the [Irvue](https://leonspok.com/irvue/landing/) app to automatically generate a new wallpaper every day and the images are so hi-res, it's quite nice.

![Unsplash Wallpapers](https://leonspok.com/irvue/landing/resources/macbook_pro.png)

### Fonts

- [Roboto](https://fonts.google.com/specimen/Roboto)
- [Roboto Mono](https://fonts.google.com/specimen/Roboto+Mono)
- [Hack](https://github.com/source-foundry/Hack)
- [Input](http://input.fontbureau.com/)

### Visual Studio Code Editor

Using [Settings Sync](https://marketplace.visualstudio.com/items?itemName=Shan.code-settings-sync) extension with this [Gist](https://gist.github.com/FrancesCoronel/42f14d19392a50ae6fd03feae51ed1de).

#### Open with Terminal

Use `Shell Command: Install 'code' command in PATH`.

![Visual Studio Code](https://i.imgur.com/NBiUCtM.png)

#### Visual Studio Code Extensions

```bash
❯ code --list-extensions | xargs -L 1 echo code --install-extension
```

- `aaron-bond.better-comments`
- `bierner.markdown-preview-github-styles`
- `christian-kohler.npm-intellisense`
- `christian-kohler.path-intellisense`
- `DavidAnson.vscode-markdownlint`
- `dbaeumer.vscode-eslint`
- `dsznajder.es7-react-js-snippets`
- `eamodio.gitlens`
- `ecmel.vscode-html-css`
- `eg2.vscode-npm-script`
- `esbenp.prettier-vscode`
- `eseom.nunjucks-template`
- `formulahendry.auto-close-tag`
- `formulahendry.auto-rename-tag`
- `GitHub.codespaces`
- `GitHub.copilot`
- `GitHub.github-vscode-theme`
- `GitHub.vscode-pull-request-github`
- `jkjustjoshing.vscode-text-pastry`
- `marvhen.reflow-markdown`
- `mdickin.markdown-shortcuts`
- `mgmcdermott.vscode-language-babel`
- `ms-vsliveshare.vsliveshare`
- `naumovs.color-highlight`
- `oderwat.indent-rainbow`
- `Orta.vscode-jest`
- `PKief.material-icon-theme`
- `redhat.vscode-yaml`
- `remimarsal.prettier-now`
- `ritwickdey.LiveServer`
- `Shan.code-settings-sync`
- `streetsidesoftware.code-spell-checker`
- `syler.sass-indented`
- `tehnix.vscode-tidymarkdown`
- `WakaTime.vscode-wakatime`
- `wayou.vscode-todo-highlight`
- `yzhang.markdown-all-in-one`
- `Zignd.html-css-class-completion`

### Homebrew

- [asciinema](https://asciinema.org/)
- [duti](http://duti.org/)
- [git](https://git-scm.com/)
- [git-lfs](https://git-lfs.github.com/)
- [howdoi](https://github.com/gleitz/howdoi)
- [hugo](https://gohugo.io/)
- [libav](https://www.libav.org/)
- [nginx](https://www.nginx.com/)
- [node](https://nodejs.org)
- [now](https://zeit.co/now)
- [openssl](https://www.openssl.org/)
- [pandoc](https://pandoc.org/index.html)
- [python](https://www.python.org/)
- [yarn](https://yarnpkg.com/en/)
- [youtube-dl](https://rg3.github.io/youtube-dl/)
- [zsh](http://www.zsh.org/)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

### macOS Apps

#### Casks

A full list of the apps installed automatically using Homebrew Casks can be found at [`init/.casks`](.init/.casks).

#### Manual

These applications don't have casks so they need to be manually downloaded from the App Store upon a fresh install.

- [Amphetamine](https://itunes.apple.com/us/app/amphetamine/id937984704?mt=12)
  - Keeps my computer on
- [BetterSnapTool](https://itunes.apple.com/us/app/bettersnaptool/id417375580?mt=12)
  - Easy to drag & resize windows
- [Day One](http://dayoneapp.com/)
  - Personal journal
- [Healthier](https://healthier.lessapps.net/)
  - Reminds me to take breaks
- [Irvue](https://apps.apple.com/us/app/irvue/id1039633667?mt=12)
  - Changes my wallpaper
- [Spark](https://sparkmailapp.com/)
  - Email client
- [SnippetsLab](https://www.renfei.org/snippets-lab/)
  - Makes it easy to reuse snippets/templates

#### Menubar

![Menubar](https://i.imgur.com/Wx12TLm.png)

### Screensaver

I use the lovely [Aerial screensaver](https://github.com/JohnCoates/Aerial) which even allows me to have different 3D views on different monitors.

![Aerial](https://aerialscreensaver.github.io/img/macbookpro-aerial.png)

### Shells

I'm using the oh-my-zsh [pure](https://github.com/sindresorhus/pure) theme.

Once the theme has loaded, you might want to replace the shell's startup command in `Preferences` under `Profiles > Shell Tab`:

`login -fpql FrancesCoronel /bin/zsh` to `login -fpql YOURNAME /bin/zsh`

#### Hyper

Copy Hyper configuration file to the root folder.

```bash
mv ~Dropbox/Code/dotfiles/bin/shell/hyper/hyper.config.js ~/.hyper.js
```

![Hyper](https://i.imgur.com/Qvej6BG.png)

#### iTerm 2

Set up sync folder in Preferences to `~/Dropbox/Code/dotfiles/bin/shell/iterm`.

![iTerm 2](https://i.imgur.com/8XcQqsh.png)

#### Terminal

Import `Materialize.terminal` profile from `~/Dropbox/Code/dotfiles/bin/shell/terminal/Materialize.terminal`.

![Terminal](https://i.imgur.com/kaqt9BC.png)

### Tracking

I use [WakaTime](https://wakatime.com/) with my [API key](https://wakatime.com/api-key) to track all the time spent across different platforms.

For editors, I have the plugin installed. Otherwise, I just use enter the following in the `~/.wakatime.cfg` file.

```text
[settings]
api_key = MY_API_KEY_GOES_HERE
```

## Theming

Accents are as follows in accordance to [Sublime Text 3 Material Theme](https://github.com/equinusocio/material-theme).

![Lime](https://img.shields.io/badge/Lime-%237CB342-lightgrey.svg?colorB=7CB342) ![Purple](https://img.shields.io/badge/Purple-%23AB47BC-lightgrey.svg?colorB=AB47BC) ![Red](https://img.shields.io/badge/Red-%23E57373-lightgrey.svg?colorB=E57373) ![Red Orange](https://img.shields.io/badge/Red_Orange-%23F74A50-lightgrey.svg?colorB=F74A50) ![Orange](https://img.shields.io/badge/Orange-%23FF7042-lightgrey.svg?colorB=FF7042) ![Yellow](https://img.shields.io/badge/Yellow-%23FFA000-lightgrey.svg?colorB=FFA000) ![Indigo](https://img.shields.io/badge/Indigo-%235C6BC0-lightgrey.svg?colorB=5C6BC0) ![Pink](https://img.shields.io/badge/Pink-%23FF4081-lightgrey.svg?colorB=FF4081) ![Blue](https://img.shields.io/badge/Blue-%232979FF-lightgrey.svg?colorB=2979FF) ![Cyan](https://img.shields.io/badge/Cyan-%2300BCD4-lightgrey.svg?colorB=00BCD4)

- Lime — `#7CB342`
- Purple — `#AB47BC`
- Red — `#E57373`
- Red orange — `#F74A50`
- Orange — `#FF7042`
- Yellow — `#FFA000`
- Indigo — `#5C6BC0`
- Pink — `#FF4081`
- Blue — `#2979FF`
- Cyan — `#00BCD4`

## Usage

If you decide to utilize these configurations, please make sure to give me some kudos as I have done below with the developers that inspired me. 😊

## Contributing

I'm very open to contributions so please feel free to

1. 🍴 [Fork this repo](https://github.com/FrancesCoronel/dotfiles#fork-destination-box)
2. 🔨 Follow the [contributing guidelines](CONTRIBUTING.md)
3. 👥 Add yourself as a contributor under the Kudos section
4. 🔧 [Make a pull request](https://github.com/FrancesCoronel/dotfiles/compare)
5. 🎉 Get your pull request approved - success!

Or just [create an issue](https://github.com/FrancesCoronel/dotfiles/issues) - any little bit of help counts! 😊

### Code of Conduct

In the interest of fostering an open and welcoming environment, we as contributors and maintainers pledge to making participation in our project and our community a harassment-free experience for everyone, regardless of age, body size, disability, ethnicity, gender identity and expression, level of experience, nationality, personal appearance, race, religion, or sexual identity and orientation.

More details can be found at this project's [code of conduct](CODE_OF_CONDUCT.md).

## Credits

- [Frances Coronel](https://github.com/FrancesCoronel) 🍓🍫

### Kudos

- [@mathiasbynens](https://github.com/mathiasbynens/dotfiles)
- [@necolas](https://github.com/necolas/dotfiles)
- [@cowboy](https://github.com/cowboy/dotfiles/)
- [@ptb](https://github.com/ptb/Mac-OS-X-Lion-Setup)
- [@pongstr](https://twitter.com/pongstr)
- [@sindresorhus](https://github.com/sindresorhus)
- [@equinusocio](https://github.com/equinusocio)
- [@agarrharr](https://github.com/agarrharr)
- [GitHub - `awesome-macOS`](https://github.com/iCHAIT/awesome-macOS)
- [GitHub - `awesome-mac`](https://github.com/jaywcjlove/awesome-mac)
- [Github - `awesome-macos-screensaver`](https://github.com/agarrharr/awesome-macos-screensaver)
- [Shields.io - README Badges](http://shields.io/)
