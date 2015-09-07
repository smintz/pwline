# pwline
powerline-like ZSH prompt designed to run on top of [YADR](https://github.com/skwp/dotfiles) and to be as flexible as possible.

## Installation
    $ git clone https://github.com/smintz/pwline ~/.pwline
    $ ln -s ~/.pwline/prompt_pwline_setup ~/.zsh.prompts/prompt_pwline_setup

#### Loading
    $ source ~/.zshrc
    $ prompt pwline

#### Personlize
    $ prompt -h pwline
    Help for pwline theme:

    This powerline prompt is customizable:

      prompt pwline [order:user,host,...] [vcsorder:vcstype,branch] [sep:<seperator char>] [colors:host:blue,white::user:green,white]

    available units options (for order:...)
      - user            - current user
      - host            - current hostname with unique background color
      - vcs             - source control information
      - time            - current clock time in 24h setup
      - jobs            - number of background jobs
      - pwd             - current directory name
      specials:
      - newline         - creates a new line
      - lastunit        - used at end of line
      - status_prompt   - terminates the prompt with red/green for last command retrun code

    available vcs units options (for vcsorder:...)
      - vcstype         - git,hg,svn,bzr
      - branch          - name of current brnach
      - revision        - full revision hash

    Type `prompt -p pwline' to preview the theme, `prompt pwline'
    to try it out, and `prompt -s pwline' to use it in future sessions.

#### Permanent setup
Add `prompt pwline` to `~/.zsh.after/prompt.zsh`
