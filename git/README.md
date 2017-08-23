# Useful Developer Git Setup

In this folder are any files that can be used to set up some useful git commands or set up git in such a way to facilitate development here at Jornaya.

## Git Config

To set up the recommended git config if you have not previously set up a git config, simply copy the `.gitconfig` file into your home directory (`~/`)

```
$ cp .gitconfig ~/
```

If you already have a git config set up, you can easily add any of the git config settings from the `.gitconfig` file in this folder by opening your `.gitconfig` file in a text editor of your choice and adding in the headings and config options manually.

```
[commit]                       <- heading
    template = ~/.gitmessage   <- config option
[alias]
    # Print a list of all current git aliases
    alias = config --get-regexp '^alias\\.'
```

## Git Commit Template

To set up the recommended git commit message template, simply copy the `.gitmessage` file into your home directory (`~/`).  Once the `.gitmessage` file is in your home directory, you can point your git config to use this template for when you are performing a commit using `git commit`.

```
$ cp .gitmessage ~/
```
If you have already copied the changes from the git config in this folder, then you will already be set up to use this git commit template, otherwise you will have to add the following to your `.gitconfig` file.

```
[commit]
    template = ~/.gitmessage
```
