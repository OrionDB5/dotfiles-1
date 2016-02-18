functions
===

## [agvim.zsh](./agvim.zsh)

agvim - Search files with ag, select with `$PERCOL`, and edit in vim.

**Usage:**

```
cd ~/Workspace/blog
agvim xmonad
```

ref) http://qiita.com/fmy/items/b92254d14049996f6ec3

## [alias.zsh](./alias.zsh)

Set aliases (if available)

**Ex)**

* apt for apt-faset
* vim for nvim
* g for git
* :q for exit
* f for thefuck
* cf-* (functions for editing some applications)
* rl-* (functions for reload some applications)

## [bindkey.zsh](./bindkey.zsh)

Bind keys

**Ex)**

* ^xe for edit in command line (useful)
* ^t for fzf-completion
* ^r for history search with fzf

## [cecho.zsh](./cecho.zsh)

cecho - colorized echo

**Usage**

```
cecho blue "Hello world!"
```

## [colorize.zsh](./colorize.zsh)

Colorize some applications outputs

* mplayer
* twitter command
* diff aliased to colordiff
* tree -C
* grep

## [command-not-found.zsh](./command-not-found.zsh)

command-not-found (available on Ubuntu)

(currently not using)

## [completion.zsh](./completion.zsh)

Set completion options

**Features**

* show completion menu
* verobose output (with description)
* ls colors with LS_COLORS

## [environment.zsh](./environment.zsh)

Set environment variables

**Features**

* language
* default application (find_alt is useful function)
* some applications options (ranger, enhancd, takenote, cheat)

## [extract.zsh](./extract.zsh)

extract - extract archive files by detecting extension

**Supported format**  
* tar.gz, tgz, tar.xz, xz, zip, lzh, tar.bz2, tbz, tar.Z, gz, bz2, Z, tar, arj

## [history.zsh](./history.zsh)

Set options for history

**Features**

* increase history size
* ignore duplicate line
* share history with each terminals

## [less.zsh](./less.zsh)

Set options for less

**Features**

* with color
* different color for bold, underline, standout font
* verbose status line message (show file name)

## [longrun-command-tracker.zsh](./longrun-command-tracker.zsh)

Notification of local host command

Automatic notification via growlnotify / notify-send  

> http://qiita.com/hayamiz/items/d64730b61b7918fbb970

"==ZSH LONGRUN COMMAND TRACKER==" is printed after long run command execution  
You can utilize it as a trigger.

## [man.zsh](./man.zsh)

man (available for buitlin commands)

> [Can I get individual man pages for the bash builtin commands? - Unix & Linux Stack Exchange](http://unix.stackexchange.com/questions/18087/can-i-get-individual-man-pages-for-the-bash-builtin-commands)
> [manpage - How to make `man` work for shell builtin commands and keywords? - Ask Ubuntu](http://askubuntu.com/questions/439410/how-to-make-man-work-for-shell-builtin-commands-and-keywords)

But I want to know about zsh builtins, so I wrote this.

Install zsh manuals to enable `man zshbuiltins`:

```
$ mkdir -p ~/Downloads/zsh-doc; cd $_
$ wget http://downloads.sourceforge.net/project/zsh/zsh/5.0.2/zsh-5.0.2.tar.bz2
$ tar -xvf zsh-5.0.2.tar.bz2
$ sudo cp Doc/*.1 /usr/local/share/man/man1
```

**Require:**

* fzf

**Optional:**

* "pygmentize" or "highlight" for highlighting scripts
* LESS="R" option for ansi color in "less" command

## [peco-history.zsh](./peco-history.zsh)

peco-select-history - for history search with ^r key

But I don't use peco now. I use fzf instead.

## [progressbar.zsh](./progressbar.zsh)

progressbar - make progress bar easily

**Usage:**

```
progressbar n [ barchar_empty barchar_fill ]
```

(int `n`: 0 ~ 100) 

> [bash - How to add a progress bar to a shell script? - Stack Overflow](http://stackoverflow.com/questions/238073/how-to-add-a-progress-bar-to-a-shell-script)

## [prompt.zsh](./prompt.zsh)

simle_is_power theme  
folked from agnoster's Theme - https://gist.github.com/3712874

In order for this theme to render correctly, you will need a
[Powerline-patched font](https://github.com/Lokaltog/powerline-fonts).

* Depends on oh-my-zsh/lib/git.zsh

TODO: make this theme standalone

## [ranger.zsh](./ranger.zsh)

ranger-cd

Compatible with ranger 1.4.2 through 1.7.*

Automatically change the directory in bash after closing ranger

This is a bash function for .bashrc to automatically change the directory to
the last visited one after ranger quits.
To undo the effect of this function, you can type "cd -" to return to the
original directory.

## [r.zsh](./r.zsh)

Start new ranger instance only if it's not running in current shell

> [ranger - ArchWiki](https://wiki.archlinux.org/index.php/Ranger#Start_new_ranger_instance_only_if_it.27s_not_running_in_current_shell)

## [shtest.zsh](./shtest.zsh)

shtest - Make testing snippet of shell script

**Usage:**

```
shtest [OPTION]
```

| Option | Arguments | Description              |
| ------ | --------- | ------------------------ |
| `-o`   | FILE      | Set the filename to edit |
| `-l`   |           | List the files           |
| `-h`   |           | Show help message        |

Require: [zsh-takenote](https://github.com/ssh0/zsh-takenote)

## [tmux.zsh](./tmux.zsh)

set tmux aliases and start up behavior

> [Start a new session from within tmux with ZSH_TMUX_AUTOSTART=true - Super User](http://superuser.com/questions/821339/start-a-new-session-from-within-tmux-with-zsh-tmux-autostart-true)

Auto start tmux when the terminal launched.

## [zgen.zsh](./zgen.zsh)

zgen load settings

* b4b4r07/enhancd zsh
* chrissicool/zsh-256color
* robbyrussell/oh-my-zsh lib/git.zsh
* robbyrussell/oh-my-zsh lib/spectrum.zsh
* robbyrussell/oh-my-zsh lib/termsupport.zsh
* robbyrussell/oh-my-zsh lib/theme-and-appearance.zsh
* ssh0/dot
* ssh0/zsh-takenote
* fcambus/ansiweather
* Tarrasch/zsh-bd
* zsh-users/zsh-syntax-highlighting

## [zplug.zsh](./zplug.zsh)

zplug load settings (not in use now)

* from oh-my-zsh
    * lib/git
    * lib/spectrum
    * lib/termsupport
    * lib/theme-and-appearance
* fcambus/ansiweather
* b4b4r07/enhancd
* b4b4r07/zplug
* Tarrasch/zsh-bd
* chrissicool/zsh-256color
* ssh0/zsh-takenote
* ssh0/dot
* zsh-users/zsh-syntax-highlighting

---

This page is generated automatically by [makebinreadme.sh](./makebinreadme.sh)
