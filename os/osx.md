# OS X Software and Settings

## Productivity

* Pomodoro timer: [Be Focused Pro](https://apps.apple.com/us/app/be-focused-pro-focus-timer/id961632517)
* Windows management: [Rectangle](https://rectangleapp.com/)

## Command Line

* Fix screw-ups in command-line: [TheFuck](https://github.com/nvbn/thefuck)
  * aliased as "please": `eval $(thefuck --alias please)`
* Shell: [zsh](../CommandLine/zsh.md)
* Terminal: [iTerm 2](https://www.iterm2.com/)
* tmux: [Tao of tmux](https://leanpub.com/the-tao-of-tmux/read)
  * tmux manager: [tmuxp](http://tmuxp.git-pull.com/en/latest/about.html)
* Package Manager: [Homebrew](https://brew.sh/)

## Dev

* JavaScript
  * nvm (aka [Node Version Manager](https://github.com/nvm-sh/nvm))
    1. `brew install nvm`
    1. Add to `.zprofile`

        ```zsh
        # You should create NVM's working directory if it doesn't exist:
        mkdir -p ~/.nvm

        # Add the following to your shell profile e.g. ~/.profile or ~/.zshrc:
        export NVM_DIR="$HOME/.nvm"
        [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
        [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
        ```
    1. Install prefered version of Node in your dev environment

       ```zsh
       nvm ls-remote --lts # This shows the LTS versions & their names
       nvm install --lts Iron
       nvm alias default lts/iron
       ```
* PHP
  * [Switching between PHP versions when using Homebrew](https://localheinz.com/articles/2020/05/05/switching-php-versions-when-using-homebrew/)
* Python
  * [Install via pyenv](https://opensource.com/article/19/5/python-3-default-mac#what-to-do)
    * Add to `.zshrc`:

      ```zsh
      # Use pyenv global version of Python
      export PYENV_ROOT="$HOME/.pyenv"
      export PATH="$PYENV_ROOT/bin:$PATH"
      if command -v pyenv 1>/dev/null 2>&1; then
        eval "$(pyenv init -)"
      fi
      ```
  
