# dev-config
开发过程中一系列工具的配置

## zsh

```
# If you come from bash you might have to change your $PATH.
# export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.
export ZSH="/Users/justinliu/.oh-my-zsh"

# Set name of the theme to load --- if set to "random", it will
# load a random theme each time oh-my-zsh is loaded, in which case,
# to know which specific one was loaded, run: echo $RANDOM_THEME
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
ZSH_THEME="robbyrussell"

# Set list of themes to pick from when loading at random
# Setting this variable when ZSH_THEME=random will cause zsh to load
# a theme from this variable instead of looking in ~/.oh-my-zsh/themes/
# If set to an empty array, this variable will have no effect.
# ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )

# Uncomment the following line to use case-sensitive completion.
# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion.
# Case-sensitive completion must be off. _ and - will be interchangeable.
# HYPHEN_INSENSITIVE="true"

# Uncomment the following line to disable bi-weekly auto-update checks.
# DISABLE_AUTO_UPDATE="true"

# Uncomment the following line to automatically update without prompting.
# DISABLE_UPDATE_PROMPT="true"

# Uncomment the following line to change how often to auto-update (in days).
# export UPDATE_ZSH_DAYS=13

# Uncomment the following line if pasting URLs and other text is messed up.
# DISABLE_MAGIC_FUNCTIONS=true

# Uncomment the following line to disable colors in ls.
# DISABLE_LS_COLORS="true"

# Uncomment the following line to disable auto-setting terminal title.
# DISABLE_AUTO_TITLE="true"

# Uncomment the following line to enable command auto-correction.
# ENABLE_CORRECTION="true"

# Uncomment the following line to display red dots whilst waiting for completion.
# COMPLETION_WAITING_DOTS="true"

# Uncomment the following line if you want to disable marking untracked files
# under VCS as dirty. This makes repository status check for large repositories
# much, much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time
# stamp shown in the history command output.
# You can set one of the optional three formats:
# "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
# or set a custom format using the strftime function format specifications,
# see 'man strftime' for details.
# HIST_STAMPS="mm/dd/yyyy"

# Would you like to use another custom folder than $ZSH/custom?
# ZSH_CUSTOM=/path/to/new-custom-folder

# Which plugins would you like to load?
# Standard plugins can be found in ~/.oh-my-zsh/plugins/*
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
plugins=(zsh-autosuggestions git)

source $ZSH/oh-my-zsh.sh

# User configuration

# export MANPATH="/usr/local/man:$MANPATH"

# You may need to manually set your language environment
# export LANG=en_US.UTF-8

# Preferred editor for local and remote sessions
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# Set personal aliases, overriding those provided by oh-my-zsh libs,
# plugins, and themes. Aliases can be placed here, though oh-my-zsh
# users are encouraged to define aliases within the ZSH_CUSTOM folder.
# For a full list of active aliases, run `alias`.
#
# Example aliases
# alias zshconfig="mate ~/.zshrc"
# alias ohmyzsh="mate ~/.oh-my-zsh"

# oh-my-zsh语法高亮效果
source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh

# nvm环境变量
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

# 设置nvm安装node的淘宝镜像
export NVM_NODEJS_ORG_MIRROR=http://npm.taobao.org/mirrors/node

#配置JDK的环境变量
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_181.jdk/Contents/Home
export PATH=$JAVA_HOME/bin:$PATH   
export CLASSPATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar 

# 配置Android SDK环境变量
export ANDROID_HOME=/Users/justinliu/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools

# 配置Flutter的国内镜像
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn

# 配置Flutter SDK环境变量
export FLUTTER_HOME=/Users/justinliu/study/Flutter/sdk/flutter
export PATH=$PATH:$FLUTTER_HOME/bin

# 配置mongodb的环境变量
export PATH=/usr/local/mongodb/bin:${PATH}


```

## VSCODE

### setting

使用 Settings Sync，使用 github 账号登录，即可下载对应的配置

### extensions

```bash
➜  ~/.vscode/extensions
➜  extensions ls

abusaidm.html-snippets-0.2.1
akamud.vscode-caniuse-0.5.3
alexisvt.flutter-snippets-2.0.0
ant-design-vue.vscode-ant-design-vue-helper-1.0.6
bang.antd-snippets-1.2.0
bierner.markdown-preview-github-styles-0.1.6
christian-kohler.path-intellisense-1.4.2
chrmarti.regex-0.2.0
cipchk.cssrem-0.1.0
codezombiech.gitignore-0.6.0
coenraads.bracket-pair-colorizer-1.0.61
dart-code.dart-code-3.5.1
dart-code.flutter-3.5.1
dbaeumer.vscode-eslint-1.9.1
donjayamanne.githistory-0.4.6
dskwrk.vscode-generate-getter-setter-0.5.0
dsznajder.es7-react-js-snippets-2.4.3
eamodio.gitlens-10.1.1
ecmel.vscode-html-css-0.2.3
editorconfig.editorconfig-0.14.2
elemefe.vscode-element-helper-0.5.6
eryouhao.brackets-light-pro-0.4.3
esbenp.prettier-vscode-2.3.0
formulahendry.auto-close-tag-0.5.6
formulahendry.auto-rename-tag-0.1.0
hollowtree.vue-snippets-0.1.11
hookyqr.beautify-1.5.0
joelday.docthis-0.7.1
jpoissonnier.vscode-styled-components-0.0.26
juliabay.spellcheck-1.1.4
kamikillerto.vscode-colorize-0.8.14
kamikillerto.vscode-colorize-0.8.15
mhutchie.git-graph-1.17.0
mkxml.vscode-filesize-2.1.3
ms-ceintl.vscode-language-pack-zh-hans-1.39.3
ms-vscode.vscode-typescript-tslint-plugin-1.2.2
msjsdiag.debugger-for-chrome-4.12.0
nash.awesome-flutter-snippets-2.0.2
naumovs.color-highlight-2.3.0
octref.vetur-0.22.4
pranaygp.vscode-css-peek-3.0.2
rubymaniac.vscode-paste-and-indent-0.0.8
russell.any-rule-0.0.7
shan.code-settings-sync-3.4.3
shd101wyy.markdown-preview-enhanced-0.4.3
spywhere.guides-0.9.3
streetsidesoftware.code-spell-checker-1.7.18
sysoev.language-stylus-1.11.0
vscode-icons-team.vscode-icons-9.4.0
wakatime.vscode-wakatime-2.2.0
wayou.vscode-todo-highlight-1.0.4
yzhang.markdown-all-in-one-2.5.1

```


