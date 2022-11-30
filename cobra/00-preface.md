---
title: "00: preface"
---

# Diving into Cobra

## Preface

This series records my personal tours into everything's source code. It won't be tutorials for anything. If you want to find some funny implements, graceful codes, this series of tours may be helpful.

As a warning, all content in this series won't judge any codes or design of these projects.

So, let's start to see what and how *Cobra* did.

## Intro

As a gopher, you must have hear the command line library *Cobra*.

*Cobra*, which is the most popular cli lib of golang, got over 29k stars in GitHub. 

## Structure

First, we determine the structure of *Cobra*.

*Cobra* contains only 14 go files and 11 go test files.

Following is summary of the content of each file.

```shell
active_help.go            # functionalities for active completion
args.go                   # arguments' validation methods, including definition of PositionalArgs
bash_completions.go       # implements of completion for bash shell
bash_completionsV2.go     # v2 implements of completion for bash shell
cobra.go                  # global methods, vars
command.go                # definition of Command, Group, including methods
command_notwin.go         # definition of a nil var preExecHookFn, which only available in windows platform
command_win.go            # definition of preExecHook, as value of preExecHookFn; This file is only built when using 'windows' build tags
completions.go            # common definitions for completion, including error, options...
fish_completions.go       # implements of completion for fish shell
flag_groups.go            # implements of flag group, including validation, utilities
powershell_completions.go # implements of completion for powershell
shell_completions.go      # common methods using for shell completion
zsh_completions.go        # implements of completion for zsh shell
```

## [Next Chapter: command](01-command.md)