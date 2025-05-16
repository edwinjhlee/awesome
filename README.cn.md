# AWESOME LIST

## Language Awesome List

| Language                              | README                                                        | Total  |
| ---                                   | ---                                                           | ---    |
| [python](https://a.x-cmd.com/python)  | [README](https://github.com/edwinjhlee/awesome/lang/python)   | 100    |
| [deno](https://a.x-cmd.com/deno)      | [README](https://github.com/edwinjhlee/awesome/lang/deno)     | 100    |
| [node](https://a.x-cmd.com/node)      | [README](https://github.com/edwinjhlee/awesome/lang/node)     | 100    |
| [bun](https://a.x-cmd.com/bun)        | [README](https://github.com/edwinjhlee/awesome/lang/bun)      | 100    |
| [java](https://a.x-cmd.com/java)      | [README](https://github.com/edwinjhlee/awesome/lang/java)     | 100    |
| [kotlin](https://a.x-cmd.com/kotlin)  | [README](https://github.com/edwinjhlee/awesome/lang/kotlin)   | 100    |


## How to contribute using Github Website

You have to login your github account.

Take `github.com/urfave/cli` as example. And and categorize it as `argument`

1. Click `Add file` then click `Create new file`. Then it will ask you to fork the project into your own github project.
2. The file path should be `cli-[urfave].yml`
3. Add the content in the following format. Then commit.

```yml
name: urfave/cli
repo: github.com/urfave/cli

desc: A simple, fast, and fun package for building command line apps in Go
desc-zh: # Optional, if you can translate it to Chinese. You can left it to blank and let the community to fill in.
```

After commit it. Then you need to create a Pull Request.

1. Go to `https://github.com/edwinjhlee/awesome/pulls`, Click `New pull request`
2. Choose the branch of your repo, then add a message.

Now you can wait for the manage dev team to review and merge it. It there is a problem, we can communicate under this PR.

TODO: add a Video demo ...

## How To contribute using PR

### Step 1: fork and clone

1. First you have to fork this repo to your own account.
2. clone this repo into your folder.

### Step 2: Change and commit

Take urfave/cli as an example. You want to add `github.com/urfave/cli` to `awesome go`, and categorize it as `argument`

You need to create a file in the folder -> `lang/go/argument`, the file name should be `cli-[urfave].yml`. If the repo is in codeberg.org, then the file should be `cli-[urfave][codeberg.org].yml`

The file is organized in yml format, which is quite simple:

```yml
name: urfave/cli
repo: github.com/urfave/cli

desc: A simple, fast, and fun package for building command line apps in Go
desc-zh: # Optional, if you can translate it to Chinese. You can left it to blank and let the community to fill in.
```

After it , you can commit. 

**[Optinal] Review the result**

You need to have [x-cmd](https://x-cmd.com) installed in your computer.
You can run `x ws gen go`. Then you can preview the newly generated go/readme.md ~



## How to contribute using ISSUE

1. Create an issue [here](https://github.com/edwinjhlee/awsome/issue), choose [new library]
2. Fill the form by providing repo name, a simple description.

This is the most simple way, however, we would prefer you contribute using PR.
