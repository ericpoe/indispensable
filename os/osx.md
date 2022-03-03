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
