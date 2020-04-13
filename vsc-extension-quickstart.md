# Welcome to your VS Code Extension

## What's in the folder

* This folder contains all of the files necessary for your extension.
* `package.json` - this is the manifest file in which you declare your language support and define the location of the grammar file that has been copied into your extension.
* `syntaxes/wbnf.tmLanguage.json` - this is the Text mate grammar file that is used for tokenization.
* `language-configuration.json` - this is the language configuration, defining the tokens that are used for comments and brackets. It's used for comment toggling etc. More details [here](https://code.visualstudio.com/api/language-extensions/language-configuration-guide)

## Get up and running straight away

* Make sure the language configuration settings in `language-configuration.json` are accurate.
* Press `F5` to open a new window with your extension loaded.
* Create a new file with a file name suffix matching your language.
* Verify that syntax highlighting works and that the language configuration settings are working.

## Test Regex

The textmate grammar fiile uses the [oniguruma](https://github.com/kkos/oniguruma) library which can be tested using [rubular](https://rubular.com/)

## Testing the syntax

[vscode-tmgrammar-test](https://github.com/PanAeon/vscode-tmgrammar-test) is used to test syntax matching. 

### Install

`npm i -g vscode-tmgrammar-test`

### Run tests

From the root of this repo:
`vscode-tmgrammar-test -c -s source.wbnf -g syntaxes/wbnf.tmLanguage.json -t \"tests/*.wbnf\"`

If you're using vscode, tests can be run using `>Tasks: Run Test Task` from the command palatte `CMD + SHIFT + P`

## Make changes

* You can relaunch the extension from the debug toolbar after making changes to the files listed above.
* You can also reload (`Ctrl+R` or `Cmd+R` on Mac) the VS Code window with your extension to load your changes.

## Add more language features

* To add features such as intellisense, hovers and validators check out the VS Code extenders documentation at https://code.visualstudio.com/docs

## Install your extension

* To start using your extension with Visual Studio Code copy it into the `<user home>/.vscode/extensions` folder and restart Code.
* To share your extension with the world, read on https://code.visualstudio.com/docs about publishing an extension.
