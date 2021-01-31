# VSCode settings

To effectively use and maintain this directory, follow the installation instructions to copy any existing vscode configurations to this directory, then create a symbolic link to point VSCode to this directory's location.

## Installation instructions (for Linux)

_WARNING_: Following these instructions will overwrite any existing custom settings in your local VSCode installation with the ones in this repo.

_Prerequisite_: Set the config directory of your VSCode installation `VSCODE_DIR` or similarly named environment variable. As of v1.52.1, this means:
```
# For Ubuntu
export VSDIR="$HOME/.config/Code/User/"
# For Mac
export VSDIR="$HOME/Library/Application\ Support/Code/User/"
```
1. Clone this repo
1. `rsync -a -v -r --ignore-existing $VSDIR .`
1. `rm -rf $VSDIR`
1. `ln -s -f -d $(pwd) $VSDIR`

## Project settings

Be wary of adding confidential information to this directory. In particular, do not add snippets containing confidential information. Use [Project snippet scope](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_project-snippet-scope) instead.

## Extensions

Note that these settings do store extensions, so when setting up a new machine, extensions will need to be reinstalled. Some useful extensions include:

- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
- [Snippet Creator](https://marketplace.visualstudio.com/items?itemName=ryanolsonx.snippet-creator)
