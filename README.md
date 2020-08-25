# VSCode settings

To effectively use and maintain this directory, follow the installation instructions to copy any existing vscode configurations to this directory, then create a symbolic link to point VSCode to this directory's location.

## Installation instructions (for Linux)

_WARNING_: Following these instructions will overwrite any existing custom settings in your local VSCode installation with the ones in this repo.

1. Clone this repo
1. `rsync -a -v -r --ignore-existing ~/.config/Code/User/ .`
1. `rm -rf ~/.config/Code/User/`
1. `ln -s -f -d $(pwd) ~/.config/Code/User/`

## Project settings

Be wary of adding confidential information to this directory. In particular, do not add snippets containing confidential information. Use [Project snippet scope](https://code.visualstudio.com/docs/editor/userdefinedsnippets#_project-snippet-scope) instead.

## Extensions

Note that these settings do store extensions, so when setting up a new machine, extensions will need to be reinstalled. Some useful extensions include:

- [Snippet Creator](https://marketplace.visualstudio.com/items?itemName=ryanolsonx.snippet-creator)
